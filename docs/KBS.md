# Koʻp Beriladigan Savollar (KBS)

---

## Nega tutuq belgisi tushirib qoldirildi?

*Agar tutuq belgisi tushirib qoldirilsa, unda Isʼhoq, daʼvo, taʼna, surʼat, sanʼat, sheʼr kabi soʻzlarda muammo boʻlmaydimi?*

### Qisqa javob

Tutuq belgisini tushirib qoldirish eng kam zararli tanlov

### Mufassal javob

Tutuq belgisi uchun 3 yechim hisobga olindi:

1. tutuq belgisini oʻzbekchada ishlatilmaydigan, lekin ASCIIʼda bor biron harf bilan almashtirish. Masalan, `c` yoki `w`: maʼno - mawno, macno, sheʼr - shewr, shecr
2. tutuq belgisini ostchiziq (`_`) bilan almashtirish: maʼno - ma_no, sheʼr - she_r
3. tutuq belgisini tushirib qoldirish

Endi birma-bir koʻrib chiqsak:

1. bu bir muammoni yechayapti, lekin menimcha, kattaroq muammoni yaratayapti. mawno, shecr - buni birdan maʼno, sheʼr ekanligini ilgʻash qiyin boʻlib qolayapti.

Buni men dasturlashdagi [mashhur gapga](https://regex.info/blog/2006-09-15/247) oʻxshataman: "Baʼzilar, muammoga duch kelganda, uni qolipli ifodalar (regex) bilan yechaman, deb oʻylaydi. Endi ularning muammosi ikkita boʻldi."

2. Bu yechim ham, agar ilonsimon nomlovdan (snake_case) foydalansangiz, qiyinchilik, noaniqlik tugʻdiradi, chunki ostchiziq boʻshliq ni bildiradi:
    yorliq_ma_nosi, navoyi_she_ri

3. Bu menimcha eng kam zararli murosa:

    a) talaffuzda tutuq belgisi yoʻqolib boʻlgan yoki yoʻqolish arafasida. Tutuq belgili soʻzlar, bular asosan arabcha ayn yoki hamza belgilari bor soʻzlarda uchraydi - koʻpchilik ularni talaffuz qilishda farqlamaydi. Oʻzingiz ham sinab koʻring, sheʼr (yozilgan) va sher (hayvon) deganingizda biron farq eshitayapsizmi.
        Men bir qancha oʻzbek domlalaridan ham eshittim: keyingi taklif qilinadigan alifbo oʻzgarishlarida tutuqni yoʻqotish. Balki bu kelajakda yuz berar.

    b) menga [Python oʻgitlaridagi](https://peps.python.org/pep-0020/#the-zen-of-python) "Soddalik murakkablikdan afzaldir" tamoyili yoqadi. Tushirib qoldirish menimcha shu tamoyilga mos keladi.

    c) `Is'hoq`, `as'hob`, `mus'haf` - bu soʻzlarni har bir oʻzbek yodlab olishi kerak. Lekin bu soʻzlar topshiriq yoki dastuvlovda ishlatilish ehtimoli kam soʻz, menimcha.

Malumingiz, dasturchilar har doim murosa qilishiga toʻgʻri keladi. Rustʼga boʻlgan muhabbatimiz ham aslida bir murosa: tezlik va xotiradan yutamiz, lekin oʻrganish muddati va murakkabligidan yutqazamiz. Xuddi maktabda oʻrganganimiz, mexanikaning oltin qoidasi bor ediku: "kuchdan yutsang masofadan yutqazasan". Xuddi shunday, tutuqni tushirib qoldirish, menimcha, eng kam zararli murosa.
