---
title: "Linux Commands"
date: 2024-06-08T08:06:25+06:00
menu:
  sidebar:
    name: Linux Commands
    identifier: linux-commands
    parent: linux
    weight: 10
hero: images/hero.jpg
tags:
- Linux
- Commands
categories:
- Basic
---

1. `Uname` - təklikdə işlədildikdə əməliyyat sisteminin adını verir (Linux), a parametri ilə işləndikdə isə əməliyyat sistemi haqqında məlumat verir: Linux kali 6.6.15-amd64 #1 SMP PREEMPT_DYNAMIC Kali 6.6.15-2kali1 (2024-04-09) x86_64 GNU/Linux
2. `Pwd` *(Print Working Directory)* – Hal hazırda hansı qovluqda olduğumuzu göstərir.
3. `Ls` *(List source*) – Bir qovluq daxilində olan hər fayl və qovluğu list şəklində göstərir. Ls – li ətraflı məlumat üçündür. Əgər orada d yazılıbsa qovluq, L yazılıbsa link, - (tire) yazılıbsa adi fayldır. Ls -a bu əmr isə hidden faylları görməyimizə kömək edir.
4. `Echo` – Text faylının içərisinə istədyimiz sözü yazdıra bilərik. Nümunə - echo “salam”>sağol - salam sözünü sağol adlı text faylının içinə yazacaq. Nümunə 2 echo salam – salam adında text faylı yaradacaq. > bu işarə yönləndirmə edir. Terminala yazı yazanda stdin, stdout və stderr bunlar icra eden fayllardər. Terminala komanda yazdıqda əgər səhvdirsə stderr (error) dan sizə mesaj gəlir. Echo salam > sagol etdikdə də eyni hadisə baş verəcək.
5. `Su` – bu əmri terminalda yazsaq bizdən şifrə istəyəcək və şifrəni düzgün daxil etdikdən sonra root səlahiyyət ilə terminalı çalışdırmağa davam edəcik.
6. `Sudo` *(Super User Do)* – Bəzi əmrlər bu əmrsiz işləmir. Super User deməkdir. Windowsdakı run as admistrator ilə eynidir deyə bilərik. Yəni root (ən yüksək) səlahiyyəti ilə əmri yerinə yetirmiş olacıq.
7. `Sudo passwd` – bu əmr isə user-in hazırki parolunu dəyişmək üçün işlədirik.
8. `Cd` *(Change Directory)* – Olduğumuz qovluqdan başqa qovluğa keçid üçün istifadə edirik. Nümunə cd .. bir üst qovluğa keçid edir, cd – isə əvvəlki qovluğa qayıdır. Cd yazıb istədiyimiz qovluğun adını yazaraqda istənilən qovluğa keçid edə bilərik. Nümudə - cd Desktop yazsaq desktopa keçəcəyik.
9. `Cat` *(Concatenate)* – Hər hansı fayl və ya sənədin içindəki textləri oxumağa imkan yaradır. Nümunə cat /etc/shells – shells-in içində nə yazıldığını göstərir bizə terminalda. Nümunə 2 - cat > salam - salam adında text faylı yaradacaq və elə terminalın içindən bu text faylının içinə nə istəsək yaza bilərik. Etdiyi digər bir şey isə, Nümünə 3 - cat salam sagol > necesen – salam və sagol faylının içərisini kopyalayır və necesen faylının içinə yapışdırır.
10. `Mv` *(Move)* – Həm qovluq və ya faylların yerini dəyişmək üçün həm də ad dəyişmək üçün işlədilir. Rename əmri olmadığı üçün bu əmrlə fayl və qovluq adını dəyişmək mümkündür. Nümunə mv salam sagol – salam adındakı qovluğun adını dəyişib sagol qoyacaq.
11. `Cp` *(copy)-* cp faylları kopyalayır, əgər qovluq kopy etmək istəyiriksə cp -r yazmalıyıq mütləq. Cp -ri yazsaq, i - bizə kopyaladığımız faylın adı ilə eydi adda fayl varsa bizdən soruşacaqki onun əvəzinə yazılsın yoxsa yox. Amma i – siz yazsaq bizdən soruşmadan kopyaladığımız şeyi avtomatik həminkinin yerinə yapışdıracaq. Cp riv – v isə ekranda nələr edildiyini göstərir. Hansı fayı hara yazıb və s. Nümunə cp -r salam sagol necesen- salam və sağol adında faylı kopyalayacaq və necesen papkasının içinə atacaq. İ,v,r işlənir bu əmrlə birlikdə. İ – info, v – etapları göstərir, r – qovluq və içindəkilərlə birlikdə kopyalamaq üçün istifadə olunur.
12. `Mkdir` *(Make Directory)* – Bir qovluq yaratmaq üçün istifadə olunur. Nümunə - mkdir kali yazsaq, kali adında qovluq yaratmış olacıq.
13. `Rmdir` *(Remove Directory)* – İçi boş qovluğu silə bilirk. Nümunə rm salam(boş qovluq) -salam adındakı qovluğu siləcək.
14. `Rm` *(Remove)* – Hər hansısa faylı silmək üçün istifadə edirik. İçərisi dolu qovluğu silmək istəsək rm -r yazmaq lazımdır. Nümunə rm salam.txt, rm -r salam (içi dolu qovluq). Rm -rv, burdadaki v isə hansı qovluqları sildiyini ekranda yazılı şəkildə bizə göstərir. Nümunə rm -r salam sagol necesen, salam və sağol adında faylı birbaşa olaraq necesen papkasının içinə atacaq.İ, v, r, f işlənir bu əmrlə birlikdə. İ – info, v – etapları göstərir, r – qovluq və içindəkilərlə birlikdə silmək üçün istifadə olunur, f – force yəni errorla qarşılaşsada məcbur silsin.
15. `Ln` *(link)* – Hardlink və softlink olmaqla iki növü var. Nümunə echo “cybernetics” > salam, salam adında text faylı yaradırıq və ln salam salam1 yazırıq. Bu əmri verdikdə 2 ədəd eyni source-u olan text faylı yaradacaq. Yəni biz salam1 dəki cybernetics sözünü silib cyber yazsaq, salam faylının içindəki olan sözdə dəyişərək cyber olacaq. Eyni fayl olur yalnız adları fərqli olur. Hard diskdədə bir dəfə yer tutur. Birini silsək digəri qalır backup kimi. Sadə ln yazsaq hardlink, ln -s yazsaq softlink yaratmış olacıq. Fərqləri isə ln -s də shortcut kimi yaradacaq, ln də isə eyni iki fayl kimi. Digər fərqi isə ln -s ilə qovluğa link vermək olur ancaq ln lə vermək olmur.
16. `Grep` *(Global Regular Expression Print)* – Bu əmr isə məsələn bir mətn olan faylda axtarış versək grep salam - həmin mətndə nə qədər salam sözü varsa onu işarəliyib bizə göstərəcək.
17. `Head` – faylda ilk 10 sətiri göstərəcək bizə. Head -n ilə biz istədiyimiz rəqəmi verə bilərik. Məsələn head -n 5 ilk 5 sətri göstərəcək. Head n 5 | wc (word count) yazsaq isə neçənci sətir, neçə söz və neçə simvoldan ibarət olduğunu göstərəcək bizə.
18. `Tail` – faylda son 10 sətri göstərəcək. Tail -n ilə biz istədiyimiz rəqəmi verə bilərik. Məsələn tail -n 5 son 5 sətri göstərəcək.
19. `Sudo apt update` – source ləri yeniləyir.
20. `Sudo apt full-upgrade -y` – update edir.