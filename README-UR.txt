Forte College of Excellence — Android starter project

یہ ایک ابتدائی Android project ہے۔ اسے ابھی حقیقی کالج کے استعمال کے لیے تیار شدہ ایپ نہ سمجھیں۔

اس میں:
- Student, Teacher اور Admin کے demo panels
- Timetable, quizzes, leave requests, attendance اور admissions کے interface cards
- موبائل پر مقامی demo entries
- GitHub Actions کے ذریعے debug APK بنانے کی workflow

اہم حدود:
- ابھی secure login موجود نہیں۔
- ابھی Firebase یا کوئی shared online database منسلک نہیں۔
- اس لیے ایک فون پر کی گئی تبدیلی دوسرے فون پر نظر نہیں آئے گی۔
- Barcode camera scanning اور حقیقی notifications ابھی شامل نہیں۔
- حقیقی طلبہ کا ذاتی ڈیٹا اس prototype میں مت ڈالیں۔

موبائل سے APK بنانے کے مراحل:
1. GitHub پر نیا repository بنائیں، مثلاً ForteCollegeApp۔
2. اس ZIP کے اندر موجود تمام files اور folders repository میں upload کریں؛ folder structure برقرار رکھیں۔
3. Repository میں Actions کھولیں۔
4. اگر workflow خود نہ چلے تو “Build Forte College APK” منتخب کرکے “Run workflow” دبائیں۔
5. کامیابی کے بعد workflow run کھولیں، نیچے Artifacts میں “Forte-College-Debug-APK” ڈاؤن لوڈ کریں۔
6. ZIP artifact extract کریں، app-debug.apk کو فون میں کھولیں اور Android کی اجازت کے مطابق install کریں۔

APK کے بعد:
اگلا کام Firebase project بنانا اور Authentication + Firestore کو منسلک کرنا ہوگا تاکہ student/teacher/admin accounts اور shared online data محفوظ طریقے سے کام کریں۔

سکیورٹی:
اپنا GitHub password یا OTP کسی کے ساتھ شیئر نہ کریں۔ حقیقی استعمال سے پہلے authentication، database security rules، backups اور testing ضروری ہیں۔
