
مايا باسل عبدالله الفئة 3
1- توصيف الحالة: 
قمت ببناء لعبة Logic Magnets على مبدأ OOP حيث قمت بتمثيل الرقعة بكلاس Board وجعلت كل خانة منه عبارة عن Object من كلاس ال Box حيث قمت باعطاء كل خانة نوع واحداثيات وقمت بأنشاء ال levels من خلال كلاس ال Levelsحيث قمت بتمرير احداثيات الخانات المطلوب ملئها بالاحجار المناسبة من مغناطيس وحديد وخلايا بيضاء 
2- فضاء الحالات :
عبارة عن الرقع الناتجة عن تحريك المغناطيس على الرقعة حيث نقوم بتحديد الموقع الجديد للمغناطيس وعند نقله سوف يتم انتاج رقعة جديدة بناءا على حركة هذا المغناطيس ان تحرك بالقرب من قطعة حديد او خانة بيضاء حيث نقوم باستدعاء توابع الحركة حسب حركة المغناطيس  
3- الحالة الابتدائية:
حيث تكون الرقعة بالبداية كما تم انشائها من خلال استدعاء الكلاسات ال Board ,Box حيث نقوم بالبداية بانشاء رقعة فارغة ثم نملؤها حسب الاحداثيات ونوع ال Box الذي تم تمريره بكلاس ال Level 
4-العمليات والاجرائيات: 
هي عبارة عن مجموعة توابع مسؤولة عن حركة القطع في الرقعة حسب اختيار المغناطيس معين لتحريك حيث توابع حركة تقوم بفحص جميع الخانات المحيطة للمغناطيس اذا كانت تحوي حديد او فارغة وتحرك الخانات المجاورة حسب التوابع وحسب المجاور لها 
5- الحالة النهائية:
لدينا حالتين يمكن ان نواجهم في الحالة النهائية ايما ان تنتهي الحركات المسموحة بها للاعب مع العلم اننا نقوم بتحقق من حالة الربح بكل انتقال حيث نرى اذا تساوى عدد الخانات البيضاء مع عدد الخانات الممتلئة 
خوارزمية ال DFS :
قمت بها من خلال تخزين الرقع المزارة ب Stack حيث كل رقعة نقوم بانشائها بسبب انتقال جديد للمغناطيس تخزن فيها ثم تنتقل الى مصفوفة ال visit لتخزينها ثم عند توليد رقعة جديدة نذهب الى ال visit لتحقق بانه تم المرور على هذه الرقعة مسبقا حيث نقارن الرقع من خلال تحويل هذه الرقعة الى مصفوفة رقمية ثم نطابق ترتيب هذه الارقام برقعة ليتم فحص اذا تم زيارة هذه الرقعة مسبقا فلم يتم زيارتها مجددا 
7- خوارزمية ال BFS :
حيث تتم على نفس مبدأ عمل ال DFS ولكن ببنية تخوين queue 
