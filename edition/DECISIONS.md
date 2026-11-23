# Editorial decisions

## Authority and scope
- **E1. Order of witnesses.** The print with the Bālamanoramā (1910) comes first, then the 1908 Nirṇaya Sāgara print, then the Kāśikā and Bālamanoramā wording. The two typed lineages (this text and ashtadhyayi-data) are not independent.
- **E2. What gets changed.** Only clear faults are corrected: typing errors, damage from old fonts, wrong numbers, and stray characters. Variant readings between prints are recorded, not imposed.
- **E3. One fault per commit.** Each commit names the SK serial, the old and new reading, and the ground.

## Spelling (from the uniformity audit)
- **U1. Nasal before a stop inside a word.** It is written as the class nasal (8.4.58).
  - A nasal at the end of a word keeps the anusvāra.
  - The entries of 8.3 and 8.4 keep both spellings, because their examples need them.
  - The Vedic and svara sections (SK 3387 on) follow the print.
- **U2. The vowel ḷ.** It is written ऌ as a full vowel and ॢ as a vowel sign, as in कॢप्त by 8.2.18 कृपो रो लः, ऌदित्, ऌकार, and ऌति ऌ वा. लृ is kept where it is l + ṛ:
  - The lakāra names लृट्, लृङ्. Their vowels after ल run a, i, u, ṛ, e, o.
  - Roots with an ṛ marker, such as वेलृ and खेलृ. These are ṛdit for 7.4.2 नाग्लोपिशास्वृदिताम्. Writing them with ॢ would make them ḷdit, and they would wrongly take aṅ by 3.1.55 पुषादिद्युताद्यॢदितः परस्मैपदेषु.
- **U3.** Jihvāmūlīya and upadhmānīya are written ᳵ and ᳶ (U+1CF5, U+1CF6).
- **U4.** Quotation marks are a plain `'`.
- **U5.** SK cross-references use ASCII digits. Devanāgarī digits remain only as Vedic accent marks.
- **U6. Old-font damage.** The damage is reversed: an i-sign typed before a conjunct (कृदि्भः → कृद्भिः) and composite glyphs (अा → आ, एे → ऐ).
- **U7. ZWNJ.** The ZWNJ after a final virāma is removed.
- **U8. Pratīka dash.** A pratīka quoted with a cross-reference is joined to the number by one hyphen (उपसर्गादृति-74). The introductory dash after अत्र भाष्यम्, तदाहुः, स्मरन्ति हि and उक्तं च is an em dash.

- **U9. Pluta and split इति.** The pluta mark is written with the Devanāgarī numeral ३ (याति३). Numerals that count repeated forms (युवाभ्याम् 3) stay in ASCII. Where an SK number split a pratīka from its इति, the full pratīka is restored and इति is written separately (घेर्ङिति 245 इति).

## Numbering
- **N1. Sūtra numbers and serial order.**
  - Sūtra numbers follow the Aṣṭādhyāyī. Twelve wrong numbers were corrected.
  - SK 3187 and 3189 were in the wrong order: अवोदैधौद्म… stands before अकर्तरि च कारके, and घञि च after it.
- **N2. Dhātu numbers.** These follow the Dhātupāṭha data, so the dhātus run 1–1992 without a gap.
  - The base had skipped 1209 (असु).
  - It had put व्रज and मार्ग under one number.
  - It had numbered केत, the variant reading after पाठान्तरम्, as a root.

## Doubtful readings (settled 2026-11-20)
- **D1. Emended** (each on grammatical ground):
  - SK 2894 वोढुं वशक्यो → वोढुं शक्यो: stray व; वोढव्यः is glossed as वोढुं शक्यः (शकि लिङ् च, 3.3.172).
  - SK 2687 उपसर्गेन समा → उपसर्गेण समा: णत्व by रषाभ्यां नो णः समानपदे (8.4.1).
  - SK 2387 इतात्वं → इतीत्वं: घुमास्थागापाजहातिसां हलि (6.4.66) gives ईत्व, read इति + ईत्वं.
  - SK 3650 अन्त्रेति → अन्यत्रेति: pratīka of the vārttika सतिशिष्टस्वरबलीयस्त्वमन्यत्र विकरणेभ्यः.
  - SK 836 र्दानीयरूपा → दर्शनीयरूपा: the series दर्शनीयकल्पा … दर्शनीयपाशा; Tattvabodhinī दर्शनीयरूपेत्यादि.
  - Dhātu 1739 अञ्चु निशेषणे → विशेषणे, and 1851 धृष प्रहसने → प्रसहने: Dhātupāṭha.
- **D2. Kept**:
  - SK 836 बहुथा: थाल् (प्रकारवचने थाल्, 5.3.23) applies to बहु under किंसर्वनामबहुभ्यः (5.3.2), after pumvadbhāva of बह्वी; the word is attested in the kośas (Apte: बहुथा "in several ways").
  - Dhātu 1735 शृधु प्रहसने: the Dhātupāṭha data itself records both प्रहसने and प्रसहने.
  - The other dhātu-name differences from the Dhātupāṭha data are notation (dental न् and छ् for the nasal and च्छ in the data) or recension variants that the Kaumudī's own forms support (बहि: बंहते; ऊर्ज, चूर्ण, घूर्ण, बिल, वल्ह, क्षिवु, रघि, दण्डनिपातने). They are the Kaumudī's readings and stay.
- **D3.** Readings reported during the encoding of SK 1680–1690: शूर्पाभ्यां (1683) and चात्वारिंशत्कः (1687) emended; त्रिंशत्कः (1689) emended from the typed त्रिंशतिकः, which has no derivation (कन् takes no इट् here; Kāśikā त्रिंशत्कः), the typed reading being kept on record here; आर्धकौडबिकम् (1685) kept, since कुडब/कुडव is a ब/व spelling variant and the Bālamanoramā spells it with ब as well.
- **D4.** SK 1409 (7.3.18): the text was emended to भद्रपादः. Both typed witnesses (this text and eBharatiSampat 524) print भाद्रपादः. That reading is rejected for three reasons. First, जे प्रोष्ठपदानाम् gives vṛddhi to the second member only (प्रोष्ठपादः), and vṛddhi of both members needs 7.3.19 ff. Second, the Kāśikā (भद्रपाद इति) reads भद्रपादः. Third, so does the Pāṇinīyamitākṣarā (भद्रपदासु जातो भद्रपादः).
- **D5.** SK 968 (6.3.10): अभ्याहितपशुः is kept. Both SK witnesses and the Pāṇinīyamitākṣarā (अभ्याहिते पशुः अभ्याहितपशुः) read it, and it is a sound counter-example to कारनाम्नि. The Kāśikā and Vasu read अभ्यर्हितपशुः, which is recorded here as a variant.
- **D6.** SK 1863 (5.2.63): emended पथिकः → पथकः. Both typed SK witnesses and the Pāṇinīyamitākṣarā print पथिकः, but वुन् gives पथकः (टिलोप 6.4.144); पथिकः is the ष्कन् form of 5.1.76. The Bālamanoramā's pratīka on this passage (पथक इति । आकादेशे नस्तद्धिते इति टिलोपः) shows the reading its author had, and the Kāśikā agrees.
- **D7.** SK 3423 (3.4.7 context, लोडर्थे लुङ्): emended तेभ्योकरं → तेभ्योऽकरं in the text and its accented copy. Both typed witnesses lack the avagraha, but अकरम् is the luṅ with the a-augment, so the sandhi needs it, and the same mantra is printed with it under SK 3406. Treated as an orthographic lapse of the print, not a variant.
- **D8.** SK 2488 (वश कान्तौ): emended the laṭ madhyama dual उष्टः → उष्ठः. Both typed witnesses (this text and eBharatiSampat 524) repeat the prathama dual उष्टः in this slot. वश् + थस् takes samprasāraṇa (6.1.16, the ending being ṅit by 1.2.4) and ष् (8.2.36), and ष्टुत्व (8.4.41) then turns थ into ठ, as in शिष्ठः under SK 2486.
- **D9.** SK 3846 (कर्णो वर्णलक्षणात्): emended शङ्कुकर्णः → शङ्कूकर्णः. This text and ashtadhyayi.com read शङ्कुकर्णः; eBharatiSampat 524 reads शङ्ककर्णः, with the vowel sign lost, so it does not decide. The lakṣaṇa word is lengthened before कर्ण by 6.3.115, शङ्कु not being among its exceptions, and the Kāśikā, the Nyāsa and the Padamañjarī on 6.2.112 all read शङ्कूकर्णः. Emended on grammatical ground with commentary support, as in D4, D6, D7 and D8.
- **D10.** SK 2573 (सूच पैशून्ये): emended the luṅ असूसुचत् → असुसूचत्. Both typed witnesses (this text and eBharatiSampat 524) read असूसुचत्. सूच is in the adanta group of the curādi (the root before it, भाम, gives अबभामत्), so 7.4.2 blocks the upadhā shortening of 7.4.1, and with a guru root syllable 7.4.93-94 do not lengthen the abhyāsa. The Kṣīrataraṅgiṇī reads असुसूचत्, the parallel adanta सूत्र in the same entry gives असुसूत्रत्. Emended on grammatical ground, as in D4 and D6-D9.
- **D11.** SK 3975 (पूजनात्पूजितमनुदात्तं काष्ठादिभ्यः): emended यत्काष्ठां → यत्काष्ठं twice (प्रपचति, शुक्लीकरोति). All three typed witnesses (this text, ashtadhyayi.com, eBharatiSampat 524) read काष्ठां. The kāṣṭhādi are a-stems used adverbially in the neuter accusative (Padamañjarī on 8.1.67: काष्ठशब्दो द्वितीयान्तः), and the Kāśikā and the Nyāsa on 8.1.68 read यत् काष्ठं in the same examples. Emended on the commentaries, as in D4 and D6-D10.
- **D12.** SK 2653 (ऋतश्च, yaṅluk of वृत्): emended the laṭ dual वर्वृतः → वर्वृत्तः (root त् + त of तस्) and the laṅ अवर्वर्तीत् → अवर्वृतीत् (7.3.87 bars guṇa before the vowel-initial pit ईत्; compare वर्वृतीति). Both typed witnesses (this text and ashtadhyayi.com) read the faulty forms; eBharatiSampat 524 is too garbled here to decide. The Vidyut forms give वर्वृत्तः and अवर्वृतीत्. The luṅ अवर्वर्तीत् is right and unchanged. Emended on grammatical ground, as in D4 and D6-D11.
- **D13.** SK 2676 (3.1.20) पुच्छभाण्डचीवराण्णिङ्: emended समवभाण्डत → समबभाण्डत. All three typed witnesses (this text, ashtadhyayi.com, eBharatiSampat 524) read समवभाण्डत. The luṅ of सम् + भाण्डि with चङ् has the abhyāsa ब (8.4.54); there is no अव in the example. The Bālamanoramā quotes समबभाण्डतेति. Emended on grammatical ground with commentary support, as in D4 and D6-D12.
- **D14.** SK 2503 (धन धान्ये): दधन्तः kept, not emended to दधान्तः. By 6.4.15 a jhal-initial ṅit तस् should lengthen the upadhā of the nasal-final stem (compare the yaṅluk शंशान्तः in the Kāśikā and दंदान्तः in the Tattvabodhinī on 6.4.15). But every witness reads दधन्तः: this text, ashtadhyayi.com, eBharatiSampat 524, the Mādhavīya Dhātuvṛtti (Mysore 1894, eBharatiSampat 634: दधन्ति दधन्तः दधनति) and Vidyut. A reading shared by an independent commentary is a reading of the tradition, not a typing fault, so it stands; the question is left for the 1910 print check and the Bālamanoramā on the root.
- **D15.** SK 3427 (लेटोऽडाटौ): emended पाताति दिद्युत् → पताति दिद्युत् (with its accented repetition). This text and ashtadhyayi.com read पाताति; eBharatiSampat 524 is garbled here. The quotation is Ṛgveda 7.25.1 पताति, given as the form without सिप्, where the pit आट् causes no vṛddhi. The Kāśikā quotes पताति दिद्युत् under 3.1.34, 3.4.7, 3.4.94 and 3.4.97. Emended on the Veda and the Kāśikā, as in D4 and D6-D13.
- **D16.** SK 2774 (न यदि): emended अभुञ्जमहि → अभुञ्ज्महि. This text and ashtadhyayi.com (with its Laghukaumudī and Bālamanoramā) read अभुञ्जमहि; eBharatiSampat 524 is garbled (अभुमहि). भुज् of the rudhādi in laṅ, uttama plural, ātmanepada: 6.4.111 श्नसोरल्लोपः drops the अ of श्नम् before the ṅit महि. The Kāśikā on 3.2.112-114, the Nyāsa and Vasu read अभुञ्ज्महि.
- **D17.** SK 2828 (समुच्चये सामान्यवचनस्य): emended याहियाहीत्ययासीति → याहियाहीत्ययासीदिति (with the Bālamanoramā; अयासीत् + इति by 8.2.39) and भुङ्ध्वम् → भुङ्ग्ध्वम् (भुज् + ध्वम्: 8.2.30 gives ग्, which nothing deletes before ध्). This text and ashtadhyayi.com share both faults; eBharatiSampat 524 lacks the passage. दाधिकमास्वादयते, also queried, is दाधिकम् आस्वादयते in sandhi and is kept.
- **D18.** SK 2887 (आसुयुवपिरपिलपित्रपिचमश्च): kept चाम्यम्, though the Kāśikā on 3.1.126 reads आचाम्यम् and 7.3.34 with the vārttika अनाचमिकमिवमीनाम् allows vṛddhi only to आङ् + चम्. This text, ashtadhyayi.com and eBharatiSampat 524 all read चाम्यम्, so the Kaumudī's own reading stands; the Kāśikā reading is noted here.
- **D19.** SK 3562 (अमो मश्): emended वंधीं वृत्रम् → वधीं वृत्रम् (with its accented repetition). This text and ashtadhyayi.com read वंधीं; eBharatiSampat 524 lacks the passage. The quotation is Ṛgveda 1.165.8 वधीम्, the luṅ of हन्/वध with इट्, as the Kaumudī's own अवधिषमिति प्राप्ते confirms; the Kāśikā on 7.1.40 reads वधीं वृत्रम्.
- **D20.** SK 2913 (कर्मण्यण्, vārttika ईक्षिक्षमिभ्यां च): kept बहुक्षामा. This text, ashtadhyayi.com and eBharatiSampat 524 all read it. The Mahābhāṣya (कल्याणक्षमा) and the Kāśikā (बहुक्षमः, बहुक्षमा) have no vṛddhi, and 7.3.34 नोदात्तोपदेशस्य मान्तस्यानाचमेः would withhold it from क्षम् in any case; the grammatical form is बहुक्षमा. As in D18, the printed Kaumudī reading stands and the correct form is recorded here.
- **D21.** SK 3608 (प्रणवष्टेः): emended जिवन्तो३म् → जिन्वतो३म् (with its accented repetition). This text and ashtadhyayi.com read जिवन्तो३म्; eBharatiSampat 524 lacks the passage. The quotation is Ṛgveda 8.44.16 जिन्वति (जिवि, इदित्, with नुम्), and the Kāśikā on 8.2.89 reads जिन्वतो३म्.
- **D22.** SK 3120 (त्रसिगृधिधृषिक्षिपेः क्नुः): kept क्षिप्नुः. This text, ashtadhyayi.com and eBharatiSampat 524 all read it. The Kāśikā on 3.2.140 reads क्षिप्णुः, which 8.4.2 अट्कुप्वाङ्नुम्व्यवायेऽपि requires (ष् of क्ष्, then इ and प् intervening); क्षिप्नु is not in the क्षुभ्नादि list (8.4.39), which has तृप्नु only. As in D18 and D20, the printed Kaumudī reading stands and क्षिप्णुः is recorded as the grammatical form.
- **D23.** SK 3264 (सङ्घोद्घौ गणप्रशंसयोः): emended इत्युद्धः → इत्युद्घः. This text and ashtadhyayi.com read उद्धः; eBharatiSampat 524 is garbled here. The word taught by the sūtra is उद्घ (घत्व by nipātana), and the Kāśikā on 3.3.86 reads उद्घो मनुष्याणाम्.

## Upstream issues (drdhaval2785/siddhantakaumudi, read 2026-11-20)
- **I1.** #74 SK 325 दादेर्धातोर्धः → दादेर्धातोर्घः (8.2.32 substitutes घ). Fixed.
- **I2.** #73 SK 311 यस्येति च number 6-4-184 → 6-4-148: already right in this text. #69 (ॠदुपध), #58 (ई३) and #71 were fixed upstream before the fork.
- **I3.** #64 special markup. The three passages had their numbers turned into SK links. Now the Liṅgānuśāsana citations read (लि १२१) and (लि १७) (त्वान्तं क्लीबम् is Liṅgānuśāsana 121 त्वष्यञौ तद्धितौ, not 120 निष्ठा च), the Māheśvarasūtra citation reads (मा.सू.-१४), and sk.json gives them as `cite` segments; the verse vārttika under SK 1088 carries `sloka: true`.
- **I4.** Not text issues, left as they are: #3 (n-gram check; superseded by the print checks here), #21 (links to dhātuvṛtti sites), #24 (DTD), #25 (CSS), #66 (Stardict placeholder).

## Open
- A second word-by-word pass against the 1910 print is still to be done, to catch faults that both typed texts share.
