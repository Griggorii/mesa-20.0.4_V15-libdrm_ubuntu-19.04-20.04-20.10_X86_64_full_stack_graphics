# mesa-20.0.4_V15-libdrm_ubuntu-20.04_and_19.04_X86_64_full_stack_graphics
graphics , mesa , 20.0.4 , libpng12 , support , x86_64 , gallium-pipe , OpenCL , d3d , nine , vdpau , libGLX_indirect , linux , ubuntu 20.04 , ubuntu 19.04 , EGL1.4 , not freeze game play steam wayland session , libc-2.31 , old stable video driver , самая лучшая в мире гамма и цветовая контрастность в браузерах , best color gamma in browsers

Ubuntu X64 ubuntu 19.04 disco dingo , ubuntu 20.04 focal fossa , Ubuntu 20.10 Groovy Gorilla , not test support ubuntu 18.10.19.10 , alternative driver libglu драйвер работает даже если вы его установите и поверх новой версии mesa тем самым заменив её.

sudo apt install libpciaccess0 -y  upgrade mesa do 20.0.4-2ubuntu1 install tar.xz

Mesa download + instructions: https://yadi.sk/d/efWd28SVdl1zJA Readme install

Example install V8 video run firefox browser : https://radikal.ru/video/37hX8285dzn

Драйвер может заработать не сразу и какое то время фризы в wayland будут выполните sudo rm -rf /var/cache/apparmor/* rm -rf ~/.cache/*

Test perfomance 2D https://www.shadertoy.com/view/3lsSzf replace my fix string compile flag rerun

News + libGLESv1 , GLU , GLX , OPENGL , libGLESv2 pkgconfig + libglu library libglu.a + libxatracker.la 01.07.2020

Test wayland video 4K and 8K https://www.youtube.com/watch?v=gYO1uk7vIcc

Внимание если вы используете мой дистрибутив гке проводником является nemo и вы обновились у вас в wayland может появиться дублирование иконок из за лиц которые тянут одеяло на себя делаем sudo -rm -rf /usr/share/gnome-shell/extensions/desktop-icons@csoriano

Если же иконки перестали появляться того же nemo значит переинсталируйте снова этот драйвер они его подменяют не заметно от пользователя по типу windows достаточно им свои ssh терминалом включить trminal=false на более медленный. На счет efi в /boot/efi/EFI/ubuntu там не должно быть лишних фаилов типа shimsshX64 всего два фаила должно быть grub.cfg и grubx64.efi


Драйвер уже фактически не тормозит в wayland видимо новый вулкан как то повлиял , а может где то что то отремонтировали и что бы не ломать структуру где была поимана эта точка то после любого обновления его наверное лучше переустанавливать именно в этой заморозке. Ранее было сильное торможение когда вкладка браузера в самом его окне не могла загрузить либо прорисовать контент иногда нельзя было переключиться на другую вкладку когда браузер был развернут полностью в размер рабочего стола в окружении wayland. Более того этот драивер работает двоекратно что усиливает качество текста и изображения как будто выставлено sRGB проверить можно запутив через терминал  nemo , nautilus либо другие программы где должно продублироваться два раза сторока вида Gtk-Message: 17:57:50.981: Failed to load module "appmenu-gtk-module" при обычном драивере эта строка не дублируется. Я пока не использовал гидру для того что бы просмотреть всю структуру и почему этот драйвер на wayland вообще идеален ещё стоит разобраться какая связь между vulkan версии 1.2.131.2 и egl1.4 что в паре получается не тормозящий работу композитор через который можно даже запустить steam и в ваших играх не будет такого дикого торможения учитывая что это wayland плюсы которого это плавность и полное отсутствие тиринга. На данный момент нету захвата видео в этом драйвере , но для тех кто может скрещивать коды есть идеяя надо посмотреть как устроен захват скриншота в коде gnome-screenshot потому что он может скринить этот композитор и сделать на основе этого библиотеку для obs-studio или green-recorder. В общем на данный момент получается с этим драйвером можно поставить убунту на телефон и он будет очень быстро работать , а запускать и гонять игры еще быстрее за счет того что размер окна мобильного телефона меньше в десятки и сотни раз , а такой драйвер работает как мне известно гораздо быстрее если экран более меньшего размера хотя там и будет у телефонов огромное разрешение.

Интересно сможет ли nvidia сделать драивер лучше пока остается в воздухе , но для работы как я понял отсюда https://github.com/NVIDIA/nvidia-docker инструменты есть , но это не к спеху я бы им посоветовал разобраться почему obs не пишет в nvenc на nvidia optimus , а потом уже лезть обгонять этот драивер который возможно быстрее и не сделаешь на wayland.

Драйвер желательно переинсталировать после каждого обновления mesa иначе можно получить торможение оболочки в wayland каждые 5-15 секунд , я пока не знаю обратили внимание на этот драйвер или просто захотят его присвоить себе никому не выдав долгожданный источник который прямо тут когда узнают что именно этого лаг тут удается почти обойти , так что как я и говорю лучше его пере инсталировать , пока это самый удачный в мире драйвер кое где в графических настройках можете выставить вертикальную синхронизацию и производительность может наоборот увеличиться , компонента драйвера гибридная по скольку тот же gles1 выключен в оригинале и какая то часть моя какая то каноникал.

Portage dump structure driver ubuntu 16.04-18.04 https://youtu.be/F5SYMzrTxjI?t=104
