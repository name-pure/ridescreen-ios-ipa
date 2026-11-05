# จอรถ iOS 1.7.0 (build 9)

iOS 15 ขึ้นไป · repository นี้มีไฟล์ติดตั้ง IPA หนึ่งไฟล์และคู่มือ ไม่มีซอร์สโค้ดแอป

[ดาวน์โหลด IPA รุ่นล่าสุด](https://github.com/name-pure/ridescreen-ios-ipa/releases/download/v1.7.0-build9/Motorcycle-Display-iOS-needs-signing.ipa)

UI ใหม่แนว Atlas ทั้ง 4 แท็บ **เชื่อมต่อ / นำทาง / Mirror / ตั้งค่า** และข้อความบนจอรถ สลับไทย/อังกฤษได้ ใช้ฟอนต์ Noto Sans Thai แบบฝังในแอป เปลี่ยนชื่อบน iPhone เป็น **จอรถ** และชื่อใน Screen Broadcast เป็น **Screen Share** ชื่อบนจอรถเริ่มต้นว่างและตั้งเองได้

คง OpenStreetMap, OpenFreeMap, Apple Maps, Wide map และ Custom การสลับแท็บหรือภาษาเก็บสถานะเชื่อมต่อและจุดหมายไว้

## ติดตั้งบน Windows

1. ดาวน์โหลด IPA ลงคอม เปิด [Sideloadly](https://sideloadly.io/) และทำตามข้อกำหนดไดรเวอร์/iTunes/iCloud จากเว็บไซต์ทางการ
2. ต่อ iPhone ผ่าน USB ปลดล็อกและกด **Trust** เลือก iPhone ใน Sideloadly
3. ลาก IPA ลง Sideloadly ใช้ Apple Account และ Bundle ID เดิมเพื่ออัปเดตทับแอปเดิม
4. **เก็บ ScreenBroadcast extension ไว้** หากมี **Remove app extensions** ให้ปิด เพื่อให้ Mirror ทำงานได้
5. กด **Start** กรอกรหัสผ่าน/รหัสยืนยันใน Sideloadly ตามที่ระบบถาม รอจนติดตั้งเสร็จ
6. หากขึ้น **Untrusted Developer:** Settings → General → VPN & Device Management → บัญชีผู้พัฒนา → Trust
7. หากขึ้น **Developer Mode Required:** Settings → Privacy & Security → Developer Mode → เปิด แล้ว Restart และยืนยัน Turn On

แตะ IPA ใน Files อย่างเดียวติดตั้งไม่ได้ บัญชีฟรีต้องเซ็นใหม่ตามอายุใบรับรอง ใช้ Auto Refresh หรือต่อคอมแล้วติดตั้งทับด้วยบัญชีเดิม ดู [FAQ ทางการ](https://sideloadly.io/faq) สำหรับเงื่อนไขและการแก้ปัญหา

## เริ่มเชื่อมต่อและนำทาง

1. เปิด **จอรถ** → แท็บ **เชื่อมต่อ** แล้วสแกน QR บนจอรถ หรือกด **วางลิงก์ QR**
2. ไป Settings → Wi-Fi เชื่อมเครือข่ายของจอรถ และเปิด Cellular Data ไว้
3. กลับแอป กด **เริ่มแสดงผล**
4. แท็บ **นำทาง** ใช้ค้นหาสถานที่ วางลิงก์ Google/Apple Maps หรือปักหมุด ตรวจจุดหมายแล้วแตะเพื่อเริ่มนำทาง
5. แท็บ **ตั้งค่า** เลือกแผนที่, 3 ส่วน / แผนที่เต็มจอ / กำหนดเอง และตั้งชื่อบนจอ เปลี่ยนไทย/EN ได้ในหัวแอปหรือหน้า Settings

## ใช้ Mirror

1. เชื่อม Wi-Fi จอรถก่อน แล้วเลือก **Mirror → เตรียมแชร์หน้าจอ / Prepare mirror** ขั้นตอนนี้หยุดแดชบอร์ดและการนำทางเดิม
2. แตะวงกลม broadcast ในแอป เลือก **Screen Share → Start Broadcast** ในหน้าต่าง iOS และรอนับถอยหลัง
3. เมื่อแชร์แล้ว ปุ่มเปิด Apple Maps, Google Maps, Waze, Spotify และ Apple Music จะใช้ได้ เปิดแอปที่ติดตั้งอยู่แล้วและควบคุมจาก iPhone หมุนแนวนอนเพื่อใช้พื้นที่จอรถมากขึ้น
4. หยุดจาก Control Center หรือกลับแอป → **หยุดแชร์หน้าจอ / Stop screen sharing**

Mirror ต้องเปิดจอและปลดล็อก iPhone ส่งเฉพาะภาพ เสียงใช้หูฟัง/อินเตอร์คอม Bluetooth การแจ้งเตือนอาจปรากฏบนจอรถ โหมดนี้ไม่ใช่ CarPlay และใช้พร้อมแดชบอร์ดไม่ได้

## นำทางขณะปิดจอ

เลือก OpenStreetMap หรือ OpenFreeMap ใน **ตั้งค่า** เปิด **นำทางขณะปิดจอ (รุ่นทดลอง)** เชื่อมต่อและเริ่มนำทางขณะเปิดแอปก่อนล็อกด้วยปุ่มด้านข้าง อย่าปัดปิดแอป Apple Maps แบบฝังยังต้องเปิดแอปนี้อยู่ด้านหน้า และ Mirror ต้องเปิดจอไว้

## การตรวจรุ่นนี้

ตรวจ build, unit tests และ UI บนตัวจำลอง iPhone/iPad ทั้งไทย/อังกฤษและสว่าง/มืดแล้ว การแชร์ข้ามแอป การติดตั้งด้วยบัญชีฟรีและการเชื่อม Zontes 368E จริง รวมถึงความหน่วง ความร้อนและแบตเตอรี่ ยังต้องทดสอบกับอุปกรณ์จริง
