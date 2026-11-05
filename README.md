RideScreen iOS 1.5.0 (build 7) · iOS 15 ขึ้นไป

ไฟล์แนบที่อัปโหลดมีเฉพาะ IPA หนึ่งไฟล์ ยังต้องเซ็นสำหรับ iPhone ด้วย Sideloadly บน Windows ก่อนติดตั้ง การแตะ IPA ในแอป Files อย่างเดียวติดตั้งไม่ได้

เพิ่ม OpenFreeMap ทั้งหน้าปักหมุดและจอรถ พร้อม Wide map, Custom และชื่อบนจอที่แก้ไขได้ โหมดปิดจอยังเป็น beta และยังไม่ได้ทดสอบภาคสนามหรือวัดความร้อนในรุ่นนี้ Apple Maps ยังต้องเปิดแอปอยู่ด้านหน้า

## ติดตั้งบน Windows
1. ดาวน์โหลดไฟล์ .ipa ใน Assets ลงคอม หากไม่เห็น Release ให้เข้าสู่บัญชี GitHub ที่เข้าถึง repository ส่วนตัวนี้ได้
2. ติดตั้งหรือเปิด [Sideloadly](https://sideloadly.io/) หากยังไม่ได้ติดตั้ง ให้ทำตามข้อกำหนด iTunes/iCloud สำหรับ Windows ที่เว็บไซต์ทางการระบุ
3. ต่อ iPhone ด้วย USB ปลดล็อก แล้วกด Trust เมื่อมีข้อความถาม เลือก iPhone ใน Sideloadly
4. ลากไฟล์ IPA ลง Sideloadly ใช้ Apple Account เดิมที่ใช้ลง RideScreen และ Bundle ID เดิม เพื่ออัปเดตทับแอปเดิม
5. เริ่มติดตั้ง กรอกรหัสผ่านและรหัสยืนยันใน Sideloadly เมื่อระบบถาม แล้วรอจนติดตั้งเสร็จ
6. หากขึ้น Untrusted Developer: Settings > General > VPN & Device Management > เลือกบัญชีผู้พัฒนา > Trust
7. หากขึ้น Developer Mode Required: Settings > Privacy & Security > Developer Mode > เปิด แล้ว Restart และยืนยัน Turn On หลังเครื่องเปิดใหม่
8. เปิด RideScreen เลือก OpenFreeMap เปิด Show the map แล้วเชื่อม Wi-Fi จอรถและกด Connect หากต้องการทดสอบล็อกจอ ให้เปิด Screen-off navigation (beta) ก่อน Connect และเริ่มนำทางขณะเปิดแอป

บัญชี Apple ฟรีต้องเซ็นใหม่ประมาณทุก 7 วัน เปิด Auto Refresh ของ Sideloadly หรือเชื่อมคอมแล้วติดตั้งทับด้วยบัญชีเดิมอีกครั้ง

หาก Sideloadly ไม่พบ iPhone ให้ตรวจว่า iTunes พบเครื่องและกด Trust แล้ว ดู [FAQ ทางการ](https://sideloadly.io/faq) สำหรับไดรเวอร์และข้อผิดพลาด

