#!url=https://raw.githubusercontent.com/manhtoi008/shad/main/modules/Locket_ohb.sgmodule
#!name=Locket-Manhtoi008_Gold
#!desc=Crack By Manhtoi008

[Script]
# ~ By Manhtoi2025
# ～ Egern transfer to Shadowrocket & Surge & LanceX
revenuecat = type=http-response, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts$|subscribers\/[^/]+$), script-path=https://raw.githubusercontent.com/manhtoi2025/shad/main/js/Locket_Manhtoi008.js, requires-body=true, max-size=-1, timeout=60

deleteHeader = type=http-request, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts|subscribers), script-path=https://raw.githubusercontent.com/Manhtoi2025/shad/main/js/deleteHeader.js, timeout=60

[MITM]
hostname = %APPEND% api.revenuecat.com
