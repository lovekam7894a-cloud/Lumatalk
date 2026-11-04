# LumaTalk — Supabase Auth edition

เพิ่มระบบสมัครสมาชิกด้วยอีเมล/รหัสผ่าน เข้าสู่ระบบ ออกจากระบบ และแสดงชื่อสมาชิกผ่าน Supabase Auth

## ตั้งค่า Supabase
1. สร้างโปรเจกต์ที่ https://supabase.com/
2. เปิด Project Settings > API หรือ API Keys
3. คัดลอก Project URL และ publishable key (หรือ anon key แบบ legacy)
4. ใน index.html แทนค่า `ใส่_SUPABASE_PROJECT_URL_ตรงนี้` และ `ใส่_SUPABASE_ANON_KEY_ตรงนี้`
5. ห้ามใส่ service_role key หรือ secret key ในเว็บไซต์
6. ใน Authentication > URL Configuration ตั้ง Site URL เป็น `https://lovekam7894a-cloud.github.io/Lumatalk/`
7. เพิ่ม URL นี้ใน Redirect URLs หากระบบร้องขอ
8. อัปโหลด index.html ฉบับใหม่ทับไฟล์เดิมใน GitHub แล้ว Commit changes

Supabase Auth จัดการรหัสผ่านให้ Publishable/anon key ใช้ใน frontend ได้ แต่ห้ามเผยแพร่ service_role/secret key ระบบแชท ห้องเสียง เหรียญ และของขวัญยังเป็นเดโม ต้องพัฒนาฐานข้อมูลและ RLS เพิ่ม
