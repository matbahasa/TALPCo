# TUFS Asian Language Parallel Corpus (TALPCo)

## Introduction
The TUFS Asian Language Parallel Corpus (TALPCo) is an open parallel corpus consisting of Japanese sentences and their translations into Burmese (Myanmar; the official language of the Republic of the Union of Myanmar), Malay (the national language of Malaysia, Singapore and Brunei), Indonesian and English.  TALPCo is licensed under a [Creative Commons Attribution 4.0 International (CC BY 4.0) license](https://creativecommons.org/licenses/by/4.0/).  See [the paper below][link] for the details of TALPCo.

## How to cite
Nomoto, Hiroki, Kenji Okano, David Moeljadi and Hideo Sawada. 2018. [TUFS Asian Language Parallel Corpus (TALPCo)][link]. Proceedings of the Twenty-Fourth Annual Meeting of the Association for Natural Language Processing.
[link]:http://www.anlp.jp/proceedings/annual_meeting/2018/pdf_dir/P3-5.pdf


## Contents

- `data_jpn.txt`	Japanese (raw sentences)

-----------------------------------

- `data_myn.txt`	Burmese (raw sentences)
- `data_myn-token.txt`	Burmese (tokenized sentences)
- `data_myn-ps.txt`	Burmese (POS-tagged sentences)

-----------------------------------

- `data_zsm.txt`	Malay (raw sentences)
- `data_zsm-token.txt`	Malay (tokenized sentences)
- `data_zsm-MWE.txt`	Malay (multiword expression list)

-----------------------------------

- `data_ind.txt`	Indonesian (raw sentences)
- `data_ind-token.txt`	Indonesian (tokenized sentences)
- `data_ind-MWE.txt`	Indonesian (multiword expression list)

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

### Burmese tokenized and POS-tagged sentences
`Sentence_ID [TAB] Sentence`

- White space: Phrasal boundary
- Dash: Morpheme boundary

    1176	မစ္စတာ-တာနာခါ-ဟာ ကျောင်းသား မ-ဟုတ်-ပါ-ဘူး ။

    1176	n-pr-postp n pref-v-suf-suf

### Malay/Indonesian tokenized sentences
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

## A note on Malay/Indonesian tokenization
The Malay and Indonesian sentences were tokenized manually by Hiroki Nomoto and David Moeljadi, respectively.  All clitics (i.e. _-nya_, _-lah_, _-kah_) were tokenized.  In addition, the instances of the prefix _se-_ were tokenized if they were an ordinal numeral.  Note that the suffix _-nya_ and the non-numeral instances of _se-_ were not tokenized.  The following dictionaries were consulted when it was not immediately obvious whether a word sequence constituted a multiword expression.

- KBBI5. 2016. [_Kamus Besar Bahasa Indonesia (edisi kelima)_](https://kbbi.kemdikbud.go.id/). Jakarta: Badan Pengembangan dan Pembinaan Bahasa.
- Nomoto, Hiroki. 2016. [_Pootaburu Nichi-Maree-Ei, Maree-Nichi-Ei Jiten \[Japanese-Malay-English, Malay-Japanese-English Portable Dictionary\]_](http://www.sanshusha.co.jp/np/details.do?goods_id=4296). Tokyo: Sanshusha.

