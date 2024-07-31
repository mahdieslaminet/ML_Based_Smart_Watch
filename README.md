# ML_Based_Smart_Watch
Machine Learning and Microcontroller based smart watch

در این پروژه به طراحی یک ساعت مچی هوشمند که قابلیت موقعیت یابی جغرافیایی و نیز اندازه گیری میزان ضربان قلب شخص تحت مراقبت و همچنین پردازش داده های مربوط به سنسور ضربان قلب و پردازش شبکه بازگشتی عمیق بر روی این داده ها و تشخیص وضعیت کنونی شخص یعنی "شخص افتاده است" و یا "شخص محصور شده است" و یا "شخص زنده است و یا مرده" و در نهایت "شخص زخمی شده است"را برعهده دارد.برای تحقق این امر از دیتاست Sisfall  و همچنین تشخیص وضعیت افتادن با کمک شبکه عصبی عمیق بازگشتی(RNN) و در نهایت ریختن مدل آموزش دیده بر روی میکروکنترلر esp32-wroom32 و پردازش داده های واقعی دریافت شده از سنسور ضربان قلب(pulse sensor) و ارسال نتیجه خروجی به محیط سرور که در این پروژه از گوگل شیت برای نمایش و ذخیره سازی داده های مربوط به موقعیت مکانی و نیز داده های مربوط به سنسور ضربان قلب و داده های مربوط به خروجی مدل آموزش دیده(یکی از 5 نوع فعالیت که مربوط به فعالیت های روزمره و نیز افتادن می باشند)،مورد استفاده قرار می گیرد.در این پروژه برای تشخیص وضعیت محصورشدگی و یا وضعیت زنده و یا مرده بودن شخص و یا تشخیص وضعیت زخمی بودن،بااستفاده از داده های مربوط به سنسور ضربان قلب که در محیط گوگل شیت قابل مشاهده می باشد،می توان این وضعیت ها را تشخیص داد.برای تشخیص وضعیت زخمی بودن شخص می توان از روی کم شدن میزان ضربان قلب این وضعیت را فهمید و یا اینکه در یک بازه زمانی وقتی موقعیت مکانی شخص تغییر نکند و مقدار ضربان قلب در حال افزایش باشد،میتوان این احتمال را داد که شخص در این موقعیت مکانی محصور شده است و در صورتی که ضربان قلب مقدارش صفر شود،به این معنی است که شخص دچار آسیستول قلبی شده است و مرده است.در این پروژه از ماژول های کم مصرف استفاده شده است که این امر باعث افزایش طول عمر باتری و منبع تغذیه مصرفی دستگاه می شود.از اینرو در این پروژه از ماژول های باتری 3.7 ولت 1000 میلی آمپرساعت جهت تغذیه دستگاه و از ماژول جی پی اس Neo6M Ublox برای تعیین موقعیت جغرافیایی و از ماژول pulsesensor همان طور که در بالا به آن اشاره شد،برای تعیین میزان ضربان قلب شخص تحت مراقبت استفاده شد.
لینک مربوط به این پروژه در ادامه آمده است و لازم به ذکر است که از زبان پایتون برای طراحی شبکه عصبی عمیق بازگشتی(RNN) و برای کدنویسی میکروکنترلر esp32-wroom32 از زبان برنامه نویسی آردوینو استفاده شده است،در آینده نه چندان دور امکان تشخیص چهار وضعیت که به آن اشاره شد،به کمک هوش مصنوعی میسر می شود.

لینک گوگل درایو توضیح پروژه طراحی مچ بند هوشمند:
https://drive.google.com/file/d/1uN2HTS5Wt-oqSwqVQp-O_pPVzVAf4x2C/view?usp=drive_link

لینک گوگل درایو پروژه و تمامی فعالیت های کلاسی:
https://drive.google.com/drive/folders/1t60cGLn013Ep5F4Ft_9nn4Ba7i-FDGYs?usp=drive_link
