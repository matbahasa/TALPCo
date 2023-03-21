# TUFS Asian Language Parallel Corpus (TALPCo)

## Introduction
The TUFS Asian Language Parallel Corpus (TALPCo) is an open parallel corpus consisting of Japanese sentences and their translations into Korean, Burmese (Myanmar; the official language of the Republic of the Union of Myanmar), Malay (the national language of Malaysia, Singapore and Brunei), Indonesian, Thai, Vietnamese and English.  TALPCo is licensed under a [Creative Commons Attribution 4.0 International (CC BY 4.0) license](https://creativecommons.org/licenses/by/4.0/).  See the paper below for the details of TALPCo.

## How to cite
- (For Korean, Burmese, Malay, Indonesian and English translations)  
Nomoto, Hiroki, Kenji Okano, David Moeljadi and Hideo Sawada. 2018. [TUFS Asian Language Parallel Corpus (TALPCo)](http://www.anlp.jp/proceedings/annual_meeting/2018/pdf_dir/C3-5.pdf). _Proceedings of the Twenty-Fourth Annual Meeting of the Association for Natural Language Processing_, 436-439.
- (For Thai and Vietnamese translations, and interpersonal meaning annotations)  
Nomoto, Hiroki, Kenji Okano, Sunisa Wittayapanyanon and Junta Nomura. 2019. [Interpersonal meaning annotation for Asian language corpora: The case of TUFS Asian Language Parallel Corpus (TALPCo)](https://www.anlp.jp/proceedings/annual_meeting/2019/pdf_dir/D4-4.pdf).  _Proceedings of the Twenty-Fifth Annual Meeting of the Association for Natural Language Processing_, 846-849. [Supplement](https://github.com/matbahasa/TALPCo/blob/master/features.pdf)
- (For Malay and Indonesian constituency tree annotations)  
Nomoto, Hiroki. 2022. [Kyokushoushugi ni motoduku heiretsu tsuriibanku no kouchiku \[Building a parallel treebank based on minimalism\]](https://www.anlp.jp/proceedings/annual_meeting/2022/pdf_dir/E1-4.pdf). _Proceedings of the Twenty-Eighth Annual Meeting of the Association for Natural Language Processing_, 103-107.

## Contents

- `data_jpn.txt`	Japanese (raw sentences)
- `data_jpn-sound.txt`	Japanese (links to sound files)
- `data_jpn-token.txt`	Japanese (tokenized sentences)
- `data_jpn-IPSpkr.csv`	Japanese (interpersonal meaning annotation, speaker)
- `data_jpn-IPAddr.csv`	Japanese (interpersonal meaning annotation, addressee)
- `data_jpn-IPLex.csv`	Japanese (interpersonal meaning annotation, lexical)
- `data_jpn-prosub.jsonl`	Japanese (pronoun substitute annotation)
- `data_jpn-prosub.txt`	Japanese (pronoun substitute annotation)

-----------------------------------

- `data_kor.txt`	Korean (raw sentences)
- `data_kor-sound.txt`	Korean (links to sound files)
- `data_kor-token.txt`	Korean (tokenized sentences)
- `data_kor-prosub.jsonl`	Korean (pronoun substitute annotation)
- `data_kor-prosub.txt`	Korean (pronoun substitute annotation)

-----------------------------------

- `data_zsm.txt`	Malay (raw sentences)
- `data_zsm-sound.txt`	Malay (links to sound files)
- `data_zsm-token.txt`	Malay (tokenized sentences)
- `data_zsm-MWE.txt`	Malay (multiword expression list)
- `data_zsm-tree.txt`	Malay (constituency tree annotation)
- `data_zsm.jpn-zsm`	Malay (partial Japanese-Malay alignment)
- `data_zsm-IPSpkr.csv`	Malay (interpersonal meaning annotation, speaker)
- `data_zsm-IPAddr.csv`	Malay (interpersonal meaning annotation, addressee)
- `data_zsm-IPLex.csv`	Malay (interpersonal meaning annotation, lexical)
- `data_zsm-prosub.jsonl`	Malay (pronoun substitute annotation)
- `data_zsm-prosub.txt`	Malay (pronoun substitute annotation)

-----------------------------------

- `data_ind.txt`	Indonesian (raw sentences)
- `data_ind-sound.txt`	Indonesian (links to sound files)
- `data_ind-token.txt`	Indonesian (tokenized sentences)
- `data_ind-MWE.txt`	Indonesian (multiword expression list)
- `data_ind-tree.txt`	Indonesian (constituency tree annotation)
- `data_ind.jpn-ind`	Indonesian (partial Japanese-Indonesian alignment)
- `data_ind-IPSpkr.csv`	Indonesian (interpersonal meaning annotation, speaker)
- `data_ind-IPAddr.csv`	Indonesian (interpersonal meaning annotation, addressee)
- `data_ind-IPLex.csv`	Indonesian (interpersonal meaning annotation, lexical)
- `data_ind-prosub.jsonl`	Indonesian (pronoun substitute annotation)
- `data_ind-prosub.txt`	Indonesian (pronoun substitute annotation)

-----------------------------------

- `data_jav.txt`	Javanese (raw sentences)
- `data_jav-prosub.jsonl`	Javanese (pronoun substitute annotation)
- `data_jav-prosub.txt`	Javanese (pronoun substitute annotation)

-----------------------------------

- `data_tha.txt`	Thai (raw sentences)
- `data_tha-sound.txt`	Thai (links to sound files)
- `data_tha-token.txt`	Thai (tokenized sentences)
- `data_tha.jpn-tha`	Thai (partial Japanese-Thai alignment)
- `data_tha-IPSpkr.csv`	Thai (interpersonal meaning annotation, speaker)
- `data_tha-IPAddr.csv`	Thai (interpersonal meaning annotation, addressee)
- `data_tha-IPLex.csv`	Thai (interpersonal meaning annotation, lexical)
- `data_tha-prosub.jsonl`	Thai (pronoun substitute annotation)
- `data_tha-prosub.txt`	Thai (pronoun substitute annotation)

-----------------------------------

- `data_vie.txt`	Vietnamese (raw sentences)
- `data_vie-sound.txt`	Vietnamese (links to sound files)
- `data_vie-token.txt`	Vietnamese (tokenized sentences)
- `data_vie-MWE.txt`	Vietnamese (multi-syllable expression list)
- `data_vie.jpn-vie`	Vietnamese (partial Japanese-Vietnamese alignment)
- `data_vie-IPSpkr.csv`	Vietnamese (interpersonal meaning annotation, speaker)
- `data_vie-IPAddr.csv`	Vietnamese (interpersonal meaning annotation, addressee)
- `data_vie-IPLex.csv`	Vietnamese (interpersonal meaning annotation, lexical)
- `data_vie-prosub.jsonl`	Vietnamese (pronoun substitute annotation)
- `data_vie-prosub.txt`	Vietnamese (pronoun substitute annotation)

-----------------------------------

- `data_myn.txt`	Burmese (raw sentences)
- `data_myn-sound.txt`	Burmese (links to sound files)
- `data_myn-token.txt`	Burmese (tokenized sentences)
- `data_myn-ps.txt`	Burmese (POS-tagged sentences)
- `data_myn-prosub.jsonl`	Burmese (pronoun substitute annotation)
- `data_myn-prosub.txt`	Burmese (pronoun substitute annotation)

-----------------------------------

- `data_eng.txt`	English (raw sentences)
- `data_eng-US.txt`	English (US) (raw sentences) \[by courtesy of [Charles Kelly](http://aitech.ac.jp/~ckelly/)\]

-----------------------------------

- `readme.me`	(this document)

## Format
All files are encoded in UTF-8 with DOS format.

### Raw sentences
`Sentence_ID [TAB] Sentence`

    1176	田中さんは 学生では ありません。
    1176	Mr Tanaka is not a student.

### Links to sound files
`Sentence_ID [TAB] URL`

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

### Burmese POS-tagged sentences
`Sentence_ID [TAB] Sentence`

- White space: Phrasal boundary
- Dash: Morpheme boundary

    1176	n-pr-postp n pref-v-suf-suf

### Constituency tree annotation
`Sentence_ID.n [TAB] bracketing` (for the `n`-th sentence for `Sentence_ID`)

    3695.2	[S [CP [Conj Tapi] [CP [C *C_decl*] [TP [DP_a [D saya]] [T'[T *T*] [AP [AP [AdvP [Adv agak]] [AP [DP *t*<a>] [A letih]]] [AdvP [Adv sedikit]]]]]]] [PU .]]

### Alignment
`Sentence_ID [TAB] Japanese_token_index-target_language_token_index`

    1176	0-1 1-0 3-3 8-2 9-4

### Interpersonal meaning annotation
See the [second paper above](#how-to-cite) and its supplement for the details of the interpersonal meaning feature system.

#### Speaker, Addressee
`Sentence_ID, Gender, Marital status, Honour, Age, Social status, Role, Group, Formality, Number`

    3243,female,,,,neutral,,,,sg

#### Lexical
`Token_index, token, Gender, Marital status, Honour, Age, Social status, Role, Group, Formality, Number`

    3845,,,,,,,,,,
    0,Cô,female,,,elder.parents_younger_sibling,,parents_sibling.paternal,,,
    1,tôi,,,,,neutral,,,,sg
    2,làm việc,,,,,,,,,
    3,ở,,,,,,,,,
    4,cửa hàng,,,,,,,,,
    5,hoa,,,,,,,,,
    6,.,,,,,,,,,
    <EOS>,,,,,,,,,,

## Notes on sound files
The sound files for the following sentences come from [TUFS Open Language Resources](https://malindo.aa-ken.jp/TUFSOpenLgResources.html#vmodwww.coelang.tufs.ac.jp/mt/vmod/).
- Japanese: All sentences except sentences 1176, 1178, 1180, 1194, 1222, 1229, 1233, 1244, 1245, 1246, 1247, 1248, 1249, 1250, 1251, 1254, 1255, 1257, 1258, 1259, 1264, 1268, 1274, 1275, 1276, 1280, 1281, 1286, 1291, 1296, 1297, 1299, 1302, 1305, 1308, 1311, 1312, 1319, 1320, 1322, 1323, 1326, 1330, 1333, 1334, 1335, 1341, 1348, 1349, 1350, 1356, 1367, 1369, 1371, 1378, 1379, 1380, 1382, 1386, 1388, 1389, 1392, 1393, 1396, 1397, 1398, 1401, 1402, 1403, 1408, 1409, 1410, 1414, 1418, 1419, 1423, 1426, 1427, 1428, 1431, 1433, 1434, 1435, 1446, 1449, 1450, 1451, 1454, 1455, 1457, 1459, 1460, 1473, 1474, 1476, 1477, 1478, 1481, 1482, 1484, 1485, 1491, 1492, 1494, 1495, 1501, 1507, 1512, 1513, 1515, 1520, 1527, 1528, 1530, 1531, 1532, 1533, 1534, 1535, 1537, 1542, 1544, 1545, 1546, 1547, 1548, 1549, 1551, 1553, 1556, 1557, 1558, 1562, 1586, 1588, 1592, 1599, 1601, 1605, 1609, 1614, 1619, 1625, 1630, 1634, 1636, 1637, 1638, 1640, 1645, 1646, 1647, 1650, 1654, 1660, 1667, 1668, 1671, 1672, 1675, 1679, 1682, 1683, 1692, 1693, 1694, 1696, 1710, 1714, 1715, 1720, 1727, 1728, 1734, 1738, 1745, 1748, 1768, 1778, 1794, 1799, 1801, 1810, 1811, 1813, 1817, 1818, 1824, 1826, 1831, 1836, 1837, 1848, 1849, 1860, 1862, 1879, 1881, 1883, 1885, 1900, 1919, 1921, 1928, 1931, 1935, 1942, 1947, 1965, 1967, 1971, 1974, 1990, 1993, 2004, 2005, 2007, 2011, 2017, 2018, 2019, 2023, 2024, 2030, 2041, 2042, 2043, 2047, 2055, 2056, 2060, 2061, 2064, 2065, 2068, 2069, 2079, 2086, 2088, 2090, 2092, 2093, 2097, 2099, 2100, 2104, 2115, 2120, 2123, 2130, 2153, 2154, 2158, 2170, 2178, 2179, 2180, 2187, 2189, 2192, 2205, 2206, 2213, 2220, 2227, 2229, 2232, 2234, 2247, 2249, 2332, 2369, 2383, 2391, 2396, 2409, 2415, 2429, 2495, 2497, 2498, 2520, 2548, 2562, 2599, 2637, 2651, 2672, 2734, 2744, 2908, 3309, 3322 and 3751.
- Malay: All sentences except sentences 1371, 1446, 1459, 2030, 2092, 2154, 2800, 2812, 3103, 3107, 3156, 3241, 3268, 3336, 3342, 3516, 3578, 3730, 3731, 3811, 3840, 3869 and 3888.
- Burmese: All sentences.

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

## Notes on pronoun substitute annotation
- See the pronoun substitute [project page](https://github.com/matbahasa/ProSub).
- One can modify the annotation, create a summary table and visualize the annotation by feeding the raw sentences and pronoun subtitute (prosub) annotation `.txt` files to [ETA: Easy Text Annotator](https://github.com/matbahasa/ETA).
