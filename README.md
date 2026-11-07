<p align="center">
  <img src="media/banner.jpg" alt="KrasWorld Launcher" width="100%">
</p>

<p align="center">
  <a href="https://github.com/ZloyPivasik/krasworld-launcher/releases/latest"><img src="https://img.shields.io/github/v/release/ZloyPivasik/krasworld-launcher?label=%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F&color=fbb6a0&labelColor=1a1330" alt="Версия"></a>
  <a href="https://github.com/ZloyPivasik/krasworld-launcher/releases"><img src="https://img.shields.io/github/downloads/ZloyPivasik/krasworld-launcher/total?label=%D1%81%D0%BA%D0%B0%D1%87%D0%B8%D0%B2%D0%B0%D0%BD%D0%B8%D0%B9&color=7c5cff&labelColor=1a1330" alt="Скачиваний"></a>
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-7c5cff?labelColor=1a1330" alt="Windows 10 и 11">
  <img src="https://img.shields.io/badge/%D0%B4%D0%B2%D0%B8%D0%B6%D0%BE%D0%BA-Rust-fbb6a0?labelColor=1a1330" alt="Движок на Rust">
</p>

<p align="center">
  <b>Лаунчер KrasWorld для Minecraft: Java Edition.</b><br>
  Свой движок на Rust, многопоточный рендер и в 2–3,5 раза больше FPS, чем у обычного Minecraft.
</p>

<p align="center">
  <a href="https://github.com/ZloyPivasik/krasworld-launcher/releases/latest/download/krasworld-launcher-setup.exe"><b>⬇ Скачать для Windows</b></a>
</p>

<p align="center">
  <img src="media/game-valley.jpg" alt="Долина с рекой и лесами на дальности прорисовки 32 чанка" width="100%">
</p>

## ✨ Чем KrasWorld особенный

- **Движок на Rust вместо Java.** Мир, рендер и игровая логика переписаны на Rust: без виртуальной машины Java и её сборщика мусора.
- **Многопоточный рендер.** Подготовка и отправка кадра идут в отдельном потоке, а невидимые куски мира отсекает видеокарта, а не процессор. В KrasWorld это включено сразу.
- **Большая дальность без мучений.** Чем дальше прорисовка, тем сильнее отрыв: на 32 чанках FPS в 3,5 раза выше, чем у обычного Minecraft.
- **Меньше памяти и быстрая загрузка.** Вдвое меньше оперативной памяти, чем у обычного Minecraft, и мир открывается почти в 4 раза быстрее.
- **Моды в пару кликов.** Каталог модов и Modrinth прямо в лаунчере, импорт сборок `.mrpack` и CurseForge.
- **Несколько сборок.** У каждой свои моды, миры и настройки.
- **Свой сервер.** Лаунчер поднимет сервер для игры с друзьями прямо с твоего компьютера.
- **Безопасность.** Вход только через аккаунт Microsoft; каждое обновление подписано ключом KrasWorld, и лаунчер не поставит файл с чужой подписью.

## 🎮 В игре

<table>
  <tr>
    <td width="50%"><img src="media/game-sunset.jpg" alt="Закат над водой и лесом"></td>
    <td width="50%"><img src="media/game-river.jpg" alt="Река среди березовых лесов"></td>
  </tr>
  <tr>
    <td width="50%"><img src="media/game-beach.jpg" alt="Песчаный берег и море"></td>
    <td width="50%"><img src="media/game-dusk.jpg" alt="Остров в вечерних сумерках"></td>
  </tr>
</table>

<sub>Все кадры сняты в KrasWorld на дальности прорисовки 32 чанка.</sub>

## ⚡ Производительность

<p align="center">
  <img src="media/fps.png" alt="График среднего FPS: Minecraft, Horizon и KrasWorld на дальности 8 и 32" width="90%">
</p>

| | Minecraft 26.3 | Horizon | **KrasWorld** |
|---|---|---|---|
| Средний FPS, дальность 8 | 944 | 1 577 | **1 973** (×2,1) |
| Средний FPS, дальность 32 | 221 | 375 | **776** (×3,5) |
| 1% худших кадров, дальность 8 | 219 | **535** | 479 |
| 1% худших кадров, дальность 32 | 47 | 111 | **174** |
| Память (RAM), дальность 32 | 2 766 МБ | 1 664 МБ | **1 210 МБ** |
| Запуск мира, дальность 8 | 27,9 с | 9,3 с | **6,8 с** |

Как мерили: один и тот же компьютер (NVIDIA RTX 4060), окно 1280×720, VSync выключен, FPS без ограничения. Новый мир с seed 1234 и четыре полёта по 12 секунд над деревней, лесом, океаном и горами; в таблице среднее по четырём сценам, по одному прогону на игру. Обычный Minecraft 26.3 запущен из своих файлов с настройками официального лаунчера (плюс загрузчик Fabric для мода, который считает кадры). На другом железе цифры будут другими.

## 🖥 Лаунчер

<table>
  <tr>
    <td width="50%"><img src="media/launcher-home.png" alt="Главная лаунчера: KrasWorld Launcher, карточки и боковое меню"></td>
    <td width="50%"><img src="media/launcher-mods.png" alt="Страница модов: каталог, Modrinth и поиск"></td>
  </tr>
</table>

## 📥 Установка

| Что | Файл | Нужно |
|---|---|---|
| Windows x64 | [`krasworld-launcher-setup.exe`](https://github.com/ZloyPivasik/krasworld-launcher/releases/latest/download/krasworld-launcher-setup.exe) | Windows 10 или 11, видеокарта с Vulkan или DirectX 12 |

1. Скачай установщик и запусти: лаунчер установится и создаст ярлык.
2. Войди через аккаунт Microsoft, на котором куплена Minecraft: Java Edition.
3. Жми **Играть**. Дальше лаунчер обновляется сам.

---

<sub>Не является официальным продуктом Minecraft. Не одобрено Mojang или Microsoft и не связано с ними.
Лицензии использованных компонентов: <a href="LICENSE">LICENSE</a>, <a href="THIRD_PARTY_NOTICES.md">THIRD_PARTY_NOTICES.md</a>, <a href="NOTICE.txt">NOTICE.txt</a>.</sub>
