# RideScreen iOS 1.6.0 (build 8)

iOS 15 ขึ้นไป · ไฟล์สำหรับติดตั้งมี IPA หนึ่งไฟล์ ไม่มีซอร์สโค้ดใน repository นี้

[ดาวน์โหลด RideScreen-Mirror-Tabs-needs-signing.ipa](https://github.com/name-pure/ridescreen-ios-ipa/raw/refs/heads/codex/ipa-only/RideScreen-Mirror-Tabs-needs-signing.ipa)

เพิ่มโหมด Mirror หน้าจอ iPhone และแยกเป็น 4 แท็บ **เชื่อมต่อ / นำทาง / Mirror / ตั้งค่า** การสลับแท็บเก็บสถานะการเชื่อมต่อและปลายทางไว้ มี OpenFreeMap, OpenStreetMap, Apple Maps, Wide map, Custom และชื่อบนจอที่แก้ไขได้ตามเดิม

## ติดตั้งบน Windows

1. ดาวน์โหลด IPA ลงคอม เปิด [Sideloadly](https://sideloadly.io/) และทำตามข้อกำหนดไดรเวอร์/iTunes/iCloud ที่เว็บไซต์ทางการระบุ
2. ต่อ iPhone ด้วย USB ปลดล็อก แล้วกด **Trust** หากมีถาม เลือก iPhone ใน Sideloadly
3. ลาก IPA ลง Sideloadly ใช้ Apple Account และ Bundle ID เดิมเพื่ออัปเดตทับแอปเดิม
4. **เก็บ ScreenBroadcast extension ไว้** หากมีตัวเลือก **Remove app extensions** ให้ปิด มิฉะนั้น Mirror จะใช้ไม่ได้
5. กด **Start** และกรอกรหัสผ่าน/รหัสยืนยันใน Sideloadly เมื่อระบบถาม รอจนติดตั้งเสร็จ
6. หากขึ้น **Untrusted Developer:** Settings → General → VPN & Device Management → บัญชีผู้พัฒนา → Trust
7. หากขึ้น **Developer Mode Required:** Settings → Privacy & Security → Developer Mode → เปิด แล้ว Restart และยืนยัน Turn On

แตะไฟล์ IPA ในแอป Files อย่างเดียวติดตั้งไม่ได้ บัญชี Apple ฟรีต้องเซ็นใหม่ประมาณทุก 7 วัน ใช้ Auto Refresh ของ Sideloadly หรือเชื่อมคอมแล้วติดตั้งทับด้วยบัญชีเดิม ดู [FAQ ทางการ](https://sideloadly.io/faq) หากหา iPhone ไม่พบหรือมีข้อผิดพลาด

## ใช้ Mirror

1. สแกน/วาง QR ในแท็บ **เชื่อมต่อ** แล้วเข้า Settings → Wi-Fi เพื่อเชื่อมเครือข่ายจอรถ เปิด Cellular Data ไว้
2. กลับเข้าแอป เลือก **Mirror → Prepare mirror** ปุ่มนี้หยุดแดชบอร์ดและการนำทางเดิม
3. แตะไอคอน broadcast ของ iOS แล้วเลือก **RideScreen Screen → Start Broadcast** รอการนับถอยหลัง
4. เมื่อเริ่มแชร์ ปุ่มเปิด Apple Maps, Google Maps, Waze, Spotify และ Apple Music จะใช้ได้ เปิดแอปที่ติดตั้งอยู่แล้วและควบคุมจาก iPhone หมุนแนวนอนเพื่อใช้พื้นที่จอรถมากขึ้น
5. หยุดผ่านตัวบันทึกหน้าจอ/Control Center หรือกลับเข้า RideScreen → **Stop screen sharing**

Mirror ต้องเปิดจอและปลดล็อก iPhone อยู่ ส่งเฉพาะภาพ เสียงออกหูฟัง/อินเตอร์คอม Bluetooth ของ iPhone การแจ้งเตือนอาจปรากฏบนจอรถ โหมดนี้ไม่ใช่ CarPlay และใช้พร้อมแดชบอร์ดไม่ได้

## ใช้นำทางแบบปิดจอ

เลือก OpenStreetMap หรือ OpenFreeMap ในแท็บ **ตั้งค่า** เปิด **Screen-off navigation (beta)** แล้ว Connect และเริ่มนำทางขณะเปิดแอป ก่อนล็อกด้วยปุ่มด้านข้าง อย่าปัดปิดแอป Apple Maps แบบฝังยังต้องเปิด RideScreen อยู่ด้านหน้า และ Mirror ไม่ใช่โหมดปิดจอ

ตรวจ build, unit tests และการสลับทั้ง 4 แท็บบนตัวจำลอง iPhone/iPad แล้ว ยังต้องทดสอบการแชร์ข้ามแอป การติดตั้งด้วยบัญชีฟรี และการเชื่อมจอ Zontes 368E จริง รวมถึงความหน่วง ความร้อนและแบตเตอรี่

