# Hydra Observatory

## О проекте / токене

HYDRA — токен Hydra в сети TON с точностью 6 знаков. Согласно самоописанию в метаданных контракта, проект ориентирован на долгосрочный фарминг: для продажи заявлены 0,66% общего объёма, остальные токены предназначены для фарминга; заявлена добыча 100 000 HYDRA в год. Это заявления проекта, а не независимо подтверждённые параметры эмиссии или доходности.

Самоописание из метаданных токена; заявления проекта не проверены независимо.

Источники (проверены 2026-11-23):

- <https://tonapi.io/v2/jettons/EQD4P32U10snNoIavoq6cYPTQR82ewAjO20epigrWRAup54_>

Generated from https://github.com/Freebielife/TON-Observatory-Template.

Run python3 -m scripts.refresh_observatory; python3 build.py; python3 verify.py.
Publish index.html in TON Sites only after independent on-chain verification.
Рыночные данные собираются из TonAPI; история расширяется постепенно. Точная полнота и актуальность разделов показаны в интерфейсе.
Only native TON swap pairs supported. Locks, staking and custom project NFT badges are configured through project.json and verified against TonAPI.
GitHub Actions настроен на 17-ю и 47-ю минуту каждого часа UTC. Фактические запуски могут задерживаться. Запись для общего Cloudflare-планировщика подготовлена в scheduler-registration.json, но не развёрнута; cron служит резервным расписанием.

Foundation version: 1.3.0. Holders show 10, expandable to top 20.
`project.json` is the per-project specification. Contract/pool/precision changes require regenerating from the factory; do not reuse another token's snapshot.
Run `python3 build.py` for an atomic bundle and `build/report.json` size report.
No external fonts, scripts or images are needed to render the saved page. Fresh data checks and manual wallet lookups require network access.
Cloudflare dispatch registration and GitHub repository access remain separate deployment steps. No credentials go into HTML.

Изображение `image(9).png` предоставлено пользователем и явно выбрано для главного баннера и всех разделов вместо флага. Источник метаданных сохранён для атрибуции, он не выдаётся за источник скачанного изображения.
