# TUFS Asian Language Parallel Corpus (TALPCo)

## Introduction
The TUFS Asian Language Parallel Corpus (TALPCo) is an open parallel corpus consisting of Japanese sentences and their translations into Burmese (Myanmar; the official language of the Republic of the Union of Myanmar), Malay (the national language of Malaysia, Singapore and Brunei), Indonesian, Thai, Vietnamese and English.  TALPCo is licensed under a [Creative Commons Attribution 4.0 International (CC BY 4.0) license](https://creativecommons.org/licenses/by/4.0/).  See the paper below for the details of TALPCo.

## How to cite
- (For Burmese, Malay and Indonesian translations)  
Nomoto, Hiroki, Kenji Okano, David Moeljadi and Hideo Sawada. 2018. [TUFS Asian Language Parallel Corpus (TALPCo)](http://www.anlp.jp/proceedings/annual_meeting/2018/pdf_dir/C3-5.pdf). _Proceedings of the Twenty-Fourth Annual Meeting of the Association for Natural Language Processing_, 436-439.
- (For Thai and Vietnamese translations, and interpersonal meaning annotations)  
Nomoto, Hiroki, Kenji Okano, Sunisa Wittayapanyanon and Junta Nomura. 2019. [Interpersonal meaning annotation for Asian language corpora: The case of TUFS Asian Language Parallel Corpus (TALPCo)]().  _Proceedings of the Twenty-Fifth Annual Meeting of the Association for Natural Language Processing_, .

## Contents

- `data_jpn.txt`	Japanese (raw sentences)
- `data_jpn-token.txt`	Japanese (tokenized sentences)

-----------------------------------

- `data_myn.txt`	Burmese (raw sentences)
- `data_myn-token.txt`	Burmese (tokenized sentences)
- `data_myn-ps.txt`	Burmese (POS-tagged sentences)

-----------------------------------

- `data_zsm.txt`	Malay (raw sentences)
- `data_zsm-token.txt`	Malay (tokenized sentences)
- `data_zsm-MWE.txt`	Malay (multiword expression list)
- `data_zsm-IPSpkr.csv`	Malay (interpersonal meaning annotation, speaker)
- `data_zsm-IPAddr.csv`	Malay (interpersonal meaning annotation, addressee)
- `data_zsm-IPLex.csv`	Malay (interpersonal meaning annotation, lexical)

-----------------------------------

- `data_ind.txt`	Indonesian (raw sentences)
- `data_ind-token.txt`	Indonesian (tokenized sentences)
- `data_ind-MWE.txt`	Indonesian (multiword expression list)
- `data_ind-IPSpkr.csv`	Indonesian (interpersonal meaning annotation, speaker)
- `data_ind-IPAddr.csv`	Indonesian (interpersonal meaning annotation, addressee)
- `data_ind-IPLex.csv`	Indonesian (interpersonal meaning annotation, lexical)

-----------------------------------

- `data_tha.txt`	Thai (raw sentences)
- `data_tha-token.txt`	Thai (tokenized sentences)
- `data_tha-IPSpkr.csv`	Thai (interpersonal meaning annotation, speaker)
- `data_tha-IPAddr.csv`	Thai (interpersonal meaning annotation, addressee)
- `data_tha-IPLex.csv`	Thai (interpersonal meaning annotation, lexical)

-----------------------------------

- `data_vie.txt`	Vietnamese (raw sentences)
- `data_vie-token.txt`	Vietnamese (tokenized sentences)
- `data_vie-MWE.txt`	Vietnamese (multi-syllable expression list)
- `data_vie-IPSpkr.csv`	Vietnamese (interpersonal meaning annotation, speaker)
- `data_vie-IPAddr.csv`	Vietnamese (interpersonal meaning annotation, addressee)
- `data_vie-IPLex.csv`	Vietnamese (interpersonal meaning annotation, lexical)

-----------------------------------

- `data_eng.txt`	English (raw sentences)

-----------------------------------

- `readme.me`	(this document)

## Format
All files are encoded in UTF-8 with DOS format.

### Raw sentences
`Sentence_ID [TAB] Sentence`

    1176	田中さんは 学生では ありません。
    1176	Mr. Tanaka is not a student.

### Tokenized sentences
`Sentence_ID [LINEBREAK] token [LINEBREAK] token [LINEBREAK] <EOS>`

    3627
    Buku
    ini
    mempunyai
    se-
    ratus
    dua
    puluh
    muka surat
    .
    <EOS>

### Burmese tokenized and POS-tagged sentences
`Sentence_ID [TAB] Sentence`

- White space: Phrasal boundary
- Dash: Morpheme boundary

    1176	မစ္စတာ-တာနာခါ-ဟာ ကျောင်းသား မ-ဟုတ်-ပါ-ဘူး ။

    1176	n-pr-postp n pref-v-suf-suf

### Interpersonal meaning annotation
#### Speaker, Addressee)
`Sentence_ID, Gender, Marital status, Honour, Age, Social status, Role, Group, Formality, Number`

#### Lexical
`Token_index, token, Gender, Marital status, Honour, Age, Social status, Role, Group, Formality, Number`

## Notes on tokenization
### Malay/Indonesian
The Malay and Indonesian sentences were tokenized manually by Hiroki Nomoto and David Moeljadi, respectively.  All clitics (i.e. _-nya_, _-lah_, _-kah_) were tokenized.  In addition, the instances of the prefix _se-_ were tokenized if they were cardinal numerals.  Note that the suffix _-nya_ and the non-numeral instances of _se-_ were not tokenized.  The following dictionaries were consulted when it was not immediately obvious whether a word sequence constituted a multiword expression.

- KBBI5. 2016. [_Kamus Besar Bahasa Indonesia (edisi kelima)_](https://kbbi.kemdikbud.go.id/). Jakarta: Badan Pengembangan dan Pembinaan Bahasa.
- Nomoto, Hiroki. 2016. [_Pootaburu Nichi-Maree-Ei, Maree-Nichi-Ei Jiten \[Japanese-Malay-English, Malay-Japanese-English Portable Dictionary\]_](http://www.sanshusha.co.jp/np/details.do?goods_id=4296). Tokyo: Sanshusha.

### Thai
The sentences were tokenized using the `tokenize` function of [Deepcut](https://github.com/rkcosmos/deepcut) and then checked by Sunisa Wittayapanyanon and Yuka Sato.  The principle adopted for the manual correction is:

- Tokenize a sequence consisting of two or more syllables if and only if all constituent syllables have a meaning that contributes to the meaning of the whole phrase/sentence.
    - Do not tokenize a sequence if it contains a meaningless syllable.
    - Do not tokenize a sequence if tokenizing it will change the meaning of the whole phrase/sentence.

### Vietnamese
The sentences were tokenized using the `word_tokenize` function of the [Undersea - Vietnamese NLP Project](http://undertheseanlp.com/) and then checked by Junta Nomura and Hiroki Nomoto.  The following dictionary was consulted when it was not immediately obvious whether a syllable sequence constituted a multi-syllable expression.

- Hoàng, Phê, ed. 2003. _Từ Điển Tiếng Việt_. Đà Nẵng: Nhà Xuất Bản Đà Nẵng.
