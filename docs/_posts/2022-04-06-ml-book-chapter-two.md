---
title: "نسخه پیش‌نویس کتاب"
date: 2022-04-06T09:18:00+03:30
categories:
  - ml
tags:
  - course
  - katex
toc: true
toc_label: "صفحات"
toc_sticky: true
---

### صفحه اول

### Neural Network and deep learning:

### AI is the new Electricity.

### What is Neural Network:

در حقیقت
Deep learning به train کردن Neural Network اشاره دارد ولی واقعا neural network چیست؟

در این قسمت با Neural Network بیشتر آشنا خواهیم شد.

با مثال معروف خودمان شروع می کنیم.
Housing price prediction
اطلاعات 6 خانه داریم و نموداری را به آن ها نسبت می دهیم که ما کمک میکند تا بتوانیم به تخمین درمورد سایر موارد (unseen data) برسیم .

<!-- -
![](../assets/images/posts/chapter-two/ch02-01.png)
- -->

\*ما می دانیم که قیمت منفی نخواهد بود لذا این قسمت از نمودار را صفر در نظر میگیریم.

حقیقت این نمودار که اینجا رسم کردیم،یک NN ساده است.شاید میتوان گفت که ساده‌ترین NN ممکن!

<!-- -
![](../assets/images/posts/chapter-two/ch02-02.png)
- -->

کاری که neuron می کند.1- سایز(x)به عنوان ورودی می گیرد. linear function -2 را حساب می کند.3- قسمت منفی را صفر در نظر می گیرد. 4- تخمین خروجی می کند.

### صفحه دوم

در مسائل NN ،این تابع را بسیار خواهیم دید:

<!-- -
![](../assets/images/posts/chapter-two/ch02-03.png)
- -->

شبکه های عصبی پیچیده تر از کنار هم قرار گرفتن و پیوند همین ساختار ساده ( single NN ) بدست می آیند.

فرض کنیم در مثال خودمان ( تخمین قیمت خانه) پارامتر های بیشتری (علاوه بر سایز) دخیل باشند.

<!-- -
![](../assets/images/posts/chapter-two/ch02-04.png)
- -->

این مثال،یک مثال فوق العادست برای درک ساعت ها فکر کردن را دارد.

نکته ی بسیار جالب در مورد NN آن است که فقط لازم است که ما تعدادی ورودی (x) و خروجی متناظر را به شبکه بدهیم و تمامی موارد دیگر توسط خود NN تنظیم میشود.

آنچه که ما در حقیقت پیاده کرده ایم چنین چیزی است.

<!-- -
![](../assets/images/posts/chapter-two/ch02-05.png)
- -->

### صفحه سوم

در حقیقت بجای آنکه ما بگوییم که neuron اول در hidden layer باید family size باشد و فقط به x1 و x2 وابسته است همه ی ورودی را در اختیار NN قرار میدهیم و خودش در مورد اینکه این NEURON چه باشد و به کدام ورودی وابسته باشد تصمیم می
گیرد.

The remarkable thing about NN is that , given enough data about x and y , (given enough training examples about x & y)
NN will be remarkably good at figuring out functions that accurately map from x to y

Supervised learning with neural networks:

در supervised learning ما یک سری ورودی x داریم و خروجی متناظر y و به دنبال آن هستیم که تابعی پیدا کنیم که این x ها را به y متناظر کند.مثل همین مثال house price

در مثال NN ، دو مفهوم وجود دارد که به توضیح آنها می پردازیم:

داده ساختاریافته(STRUCTURED DATA):در این نوع دیتا هر یک از feature های ورودی ساختار منظمی دارند مثل:

<!--- ![](../assets/images/posts/chapter-two/ch02-06.png) --->

### صفحه چهارم

سوالی که پیش می آید آن است که اگر ایده ی NN دهه ها پیش مطرح شده است چرا اخیرا اینقدر مورد توجه قرار گرفته است؟

<!--- ![](../assets/images/posts/chapter-two/ch02-07.png) --->

در این روش ها،تا جایی با افزودن data جدید،performance بالاتر میرود ولی از جایی به بعد در حقیقت اشباع میشود و افزودن data جدید تاثیری بر کارایی سیستم ندارد.

اتفاقی که در حدود ۲۰ سال گذشته رخ داده آن است که ما از یک حجم کم از اطلاعات حجم بسیار زیادی از داده رسیده ایم و این مساله بخاطر digitalization است.

در حقیقت به نقطه ای رسیدیم که حجم بسیار خوبی از اطلاعات را ببینیم ولی روش های مرسوم قادر نبودند از آن برای بهبود کارایی استفاده کنند.

و بنابراین اگر performance در این حد میخواهیم به ۲ موضوع نیاز داریم:

۱.یک NN نسبتا بزرگ

۲.یک حجم بسیار وسیع از اطلاعات

نتیحه از 1و2:
فراهم کردن این ۲ پارامتر به معنای نیاز به امکانات سخت افزاری و نرم افزاری پیچیده است که تنها در همین چند سال اخیر فراهم شده است.

### صفحه پنجم

در حقیقت منظور از Amount of Data که روی محور x نمودار مشخص شده Amount of Labeled Data است (x,y) که در آن ورودی و خروجی متناظر برای dataset مشخص،معین شده است.

#training examples⇐(m)

نکته‌ی بعدی آنست در جایی که small training set داریم،ممکن است حتی روش‌های قدیمی (,...SUM) بهتر از یک large NN به شدت قوی‌تر عمل می کند.

پارامترهایی که پیش از این باعث پیشرفت NN شده‌اند،دسترسی بیشتر به Data و Computation بوده است حال آن که در سال‌های اخیر استفاده از Algorithm های جدید،مورد توجه است.

\*این الگوریتم ها در سرعت بخشی به NN بسیار موثر بوده‌اند.یکی از ساده‌ترین مثال‌ها در این زمینه ، سوییچ از Sigmoid به relu بوده است.

<!--- ![](../assets/images/posts/chapter-two/ch02-08.png) --->

در این قسمت ها،شیب بسیار کم است و gradiene هم بسیار کم (تقریباً صفر) است و بنابراین learning بسیار کندی میشود.

### صفحه ششم

یکی دیگر از دلایلی که سرعت الگوریتم ها اینقدر برای ما مهم است آن است که مهمولاً در پیاده سازی الگوریتم‌ها این چرخه طی میشود. ابتدا ایده‌ای داریم
این ایده تبدیل به کد می‌شود.
کد را امتحان میکنیم.

<!--- ![](../assets/images/posts/chapter-two/ch02-09.png) --->

در این فرایند سرعت بسیار مهم است.

Logistic Regression as a Neural Network -Binary Classification:

در این هفته در مورد مبانی NN صحبت خواهیم کرد:
برای پیاده سازی یک NN، مجموعه‌ای از تکنیک‌ها وجود دارد که بهره‌گیری از آن‌ها به افزایش کارایی NN کمک خواهد کرد.
مثلاً اجتناب از بکار بردن حلقه‌ی for در پیاده‌سازی الگوریتم‌ها.

الگوریتم Logistic regression برای binary classification است.

Binary Classification

<!--- ![](../assets/images/posts/chapter-two/ch02-10.png) --->

میدانیم که هر تصویر RGB از سه ماتریس تشکیل شده. حال فرض کنیم عکس در ابعاد 64\*64 داریم.

در این حالت در حقیقت 64\*64\*3 تا مقدار داریم.برای آنکه این مقادیر را به یک feature vector تبدیل کنیم، همه را به یک بردار عمودی تبدیل میکنیم.

### صفحه هفتم

<!--- ![](../assets/images/posts/chapter-two/ch02-11.png) --->

Notation is so important

بعضی وقت ها از n برای بیان ابعاد ورودی استفاده میشود.

Notation:
A single training example is represented by (x,y)

<!--- ![](../assets/images/posts/chapter-two/ch02-12.png) --->

همچنین از M train و M test هم برای بیان تعداد مثال های موجود در هر مجموعه استفاده میشود.

### صفحه هشتم

یکی از روش های مرسوم برای نمایش training examples این است :

<!--- ![](../assets/images/posts/chapter-two/ch02-13.png) --->

در حقیقت هر یک از m مثال training را در یک ستون قرار میدهیم.

<!--- ![](../assets/images/posts/chapter-two/ch02-14.png) --->

Logistic regression:

یکی از learning algorithm هایی است که در مسائل binary classification استفاده میشود.جایی که خروجی یا صفر خواهد بود و یا یک.

فرض کنیم یک ورودی x داریم مثلا یک تصویر که میخواهیم ببینیم آیا در آن گربه هست یا خیر؟

و می خواهیم یک prediction داشته باشیم (y^)

که در حقیقت تخمین ما از y است.

در حقیقت y^ ، احتمال آن است که y=1 باشد وقتی که ورودی برابر با x است.

<!--- ![](../assets/images/posts/chapter-two/ch02-15.png) --->

### صفحه نهم

به بیان دیگر، اگر x یک تصویر ورودی باشد، y به ما میگوید چقدر احتمال دارد که تصویر آن ، تصویر یک گربه باشد.

همانطور که پیش‌تر گفتیم x ابعادی با Nx دارد. Rnxx با توجه به این موضوع پارامترهای logistic regression یا همان W:

Parametrs: WRnx , bR

در این جا b یک عدد حقیقی است.

به نظر میرسه داریم فقط درمورد یک neuron در هر لایه صحبت می کنیم.

<!--- ![](../assets/images/posts/chapter-two/ch02-16.png) --->

فرض کنیم ورودی x را داریم،همچنین پارامترهای W,b را هم داریم،چگونه y تولید می شود.

<!--- ![](../assets/images/posts/chapter-two/ch02-17.png) --->

دلیل استفاده از آن است که ما می خواهیم y بیانگر احتمال باشد، یعنی عددی بین صفر و یک.

<!--- ![](../assets/images/posts/chapter-two/ch02-18.png) --->

### صفحه دهم

در استفاده از logistic regression ، هدف ما پیدا کردن w و b مناسب است بطوریکه y^ احتمال درستی باشد.
برای فرآیند learning و train کردن b,w قبل از هرچیز نیاز به یک cost function داریم که در این قسمت به آن میپردازیم:
گفتیم که :

<!--- ![](../assets/images/posts/chapter-two/ch02-19.png) --->

از طرفی ما مجموعه ای از m تا training examples داریم:

<!--- ![](../assets/images/posts/chapter-two/ch02-20.png) --->

Loss(error) function:

<!--- ![](../assets/images/posts/chapter-two/ch02-21.png) --->

این یکی از روش هایی است که میتوانیم از آن استفاده کنیم (squared-error)
ولی در logistic regression معمولا از این فرمول استفاده نمیشود.
چرا که کار با آن در optimization که بعدا در مورد آن حرف میزنیم،آسان نیست.
در حقیقت loss function ابزار ماست برای آن که دریابیم تا چه حد تخمین ما y^ درست بوده و به واقعیت y نزدیک بوده است.

### صفحه یازدهم

آنچه که ما از آن به عنوان loss function استفاده می کنیم این است طبیعتاً خواسته‌ی ما این است که فارغ از هر تابعی که برای loss استفاده می کنیم،مقدار آن کمترین مقدار ممکن باشد.

L(y^,y)=-(y log y^ + (1-y)log(1-y^))
If y=1⇒ L (y^,y)=-logy^

این یعنی اگر y=1 باشد، ما ترجیح می دهیم که y^ تا حد ممکن بزرگ باشد تا که loss کم شود.

از سوی دیگر بزرگ ترین مقدار ممکن برای y^ معادل با یک(1) است پس وقتی که y=1 است، y^=1 خواهد بود.

If y=o ⇒L(y^-y)=-log (1-y^)

بنابراین ترجیح ما این است که (log(1-y تا حد ممکن بزرگ باشد پس (y-1) باید بزرگ باشد پس y^ باید کمترین مقدار را داشته باشد. لذا:y^=0

نکته‌ی آخر اینکه تا اینجا training examples بیان شده است.

در اینجا ما Cost function را تعریف میکنیم که در حقیقت به ما میگوید چقدر خوب باید عمل کرده‌ایم روی مجموعه کامل training set

<!--- ![](../assets/images/posts/chapter-two/ch02-22.png) --->

### صفحه دوازهم

### صفحه سیزدهم

خب ، تا اینجا کاری که کردیم این بوده که پیکسل به پیکسل یک تصویر را بررسی کردهایم.مثلاً گفتهایم این پیکسل 10 هست این پیکسل127 و...
در Convolutional Neural Network ، کمی کلی تر به قضیه نگاه میکنیم.در حقیقت به دنبال feature هایی در تصویر در میگردیم.مثلاً یک بندکفش و یک کف کفش یعنی کفش.این کار را با اعمال فیلترهای مختلف به تصویر انجام میدهیم. هر فیلتر برای آشکارسازی یک feature است.
Week3:
What are calvolutions and pooling?
همانطور که گفتیم تا اینجا ما توانستهایم DNN بسازیم و از آن برای تشخیص Fashion-MNIS1 و MNIS1 استفاده کنیم. کاری که تا اینجا کردهایم Pixel-wise بوده. یعنی پیکسل به پیکسل تصاویر را بررسی کردهایم و راجع به هریک تصمیم گرفتیهایم. 764 پیکسل در هر تصویر؛ سوالی که میخواهیم جواب دهیم این است که: آیا امکان دارد که تصویر را کنسانتره (چکیده) کرد بطوریکه فقط feature های مهم بررسی شوند؟! Convolution این کار را انجام میدهد. در هر تصویر قسمتهای اضافه وجود دارد که الزاماً اطلاعات خاصی به ما نمیدهد.
Convolution در حقیقت در نظر گرفتن فیلترهای مختلف و اعمال آنها بر کل تصویر است.
ایدهی کلی آنست که با درنظر گرفتن فیلترهای مناسب،خروجی تولید کنیم که در آن برخی feature ها نمایان باشند.
اگر convolution را با مفهومی به نام pooling ترکیب کنیم به الگوریتم بسیار قدرتمندی میرسیم.
\*pooling در حقیقت روشی برای compress کردن یک تصویر است. یکی از سادهترین روشهای pooling، nm pooling است که در آن بزرگترین عدد از هر 4 تا پیکسل همسایه انتخاب میشود.

### صفحه چهاردهم

```ruby

Tmplementing Convolutional layers:

model=tf.keras.models.sequential ([tf.keras.layers-ConvZD(64,(3,3),activation=’relu’,input- shape=(28,27,1)),

tf.keras.layers.MaxPooling ZD (2,2),

tf.keras.layers.Conv ZD(64,(3,3),oc…. =’relu’)
tf.keras.layers.MaxPooling ZD(2,2)

tf.keras.layers.Flattenc…,
tf.keras.layers.Dense(128,activation=’relu’),
tf.keras.layers.Dense(10,activation=’so….’)

```

*سه خط آخرش همان است که پیش تر داشتیم.  
1- در اینجا به keras میگوییم که 64 فیلتر را برای ما درنظر بگیرد سایز هر پیکسل 3*3 است. activationهست یعنی مقادیر منفی نادیده گرفته میشود و input-hope هم ....
2- برای هر پیکسل مجاور، بزرگترین مقدار به عنوان خروجی در نظر گرفته میشود.
3- سپس یک لایهی دیگر از pooling layer,Convolutional اضافه شده است.
بنابراین تا قبل از اینکه تصویر به flatten برسد، کوچک و کوچکتر شده و اطلاعات اضافی آن حذف شده است.
Model summary ( )
ابزار بسیار مفیدی است که اطلاعات بسیار خوبی راجع ....

### صفحه پانزدهم

Output shape
(none,2b,2b,b4)
Output size=( n+2p-fs+1)(n+2p-fs+1)

طبیعتا با افزودن 2 لایه ی pooling convolution ، سرعت پردازش کاهش یابد.
اتفاقی که می افتد این است:
برای هر تصویر ،b4 فیلتر در نظر گرفته میشود و سپس تصویر compress میشود و دوباره b4 فیلتر اعمال میشود و دوباره تصویرcompressمیشود و سپس حاصل به DNN اعمال میشود و این اتفاق برای 60000 تصویر می افتد در هر epoch
خب حالا به سراغ یک تمرین میرویم و سعی میکنیم با تغییر پارامتر های مختلف تاثیر هر یک را بررسی کنیم.
خب مرحله به مرحله پیش میرویم چیزی که پیش از اعمال CNN داشتیم یک DNN بود که نتایج به ترتیب هستند.(GPU)

Training= acc=0.8934
Loss=0.2911
Testing= acc=0.8813
Loss=0.3348
Total time/epoch=>5s,90 µ.s
حالا ، convolution neural netwr را به DNN اضافه میکنیم.

Training= acc=0.9285
Loss=0.1925
Testing= acc=0.9048
Loss=0.2662
Total time/epoch=>13s,211 µ.s
نکته بسیار مهمی در مورد کدنویسی CNN وجود دارد.
Training \_images=training_images.reshape (60000,28,28)
Test_images=test_images.reshape(10000,28,28)
That `s because the first convolution expects a single tensor containing everything so instead of 60000 28×28×1 items in a list ,are have a single 4D lost + hot is 60000 ×28×28×1

### صفحه شانزدهم

خب بریم سراغ بررسی حالت اولیه:

```ruby
Training= acc=0.93
Loss=0.1871
Testing= acc=0.91
Loss=0.25
Time=13s
```

حالا به جای 64،32 در نظر میگیریم

```ruby
Training= acc=0.9195
Loss=0.2178
Testing= acc=0.90
Loss=0.26
Time=10s
```

حالا16:

```ruby
Training= acc=0.90
Loss=0.26
Testing= acc=0.82
Loss=0.29
Time=9s
```

حالا convolution اخر را برمیداریم.

```ruby
Training= acc=0.85
Loss=0.37
Testing= acc=0.90
Loss=0.26 time=11s
```

حالا یک لایه اضافه تر میکنیم.=> چرا؟ شاید سایز تصویر زیاد کوچک شد.

```ruby
Training= acc=0.86
Loss=0.37
Testing= acc=0.85
Loss=0.41

```

Week4
خب تا اینجا عالیه !من تونستم یک CNN را برای mnist و fasion mnist پیاده سازی کنم .نکته ای که وجود دارد این است که تصاویر موجود در این دیتاست ها کم حجم (28×28) هستند و همچنین objectها در مرکزشان قرار دارد.حالا میخواهیم وارد پروژه های پیچیده تر شویم.

### صفحه هفدهم

تا اینجا دیدیم که چگونه میتوانیم یک classifier با DNN درست کنیم و چگونه کارایی آن را با افزودن DNN بهبود ببخشیم.
یکی از محدودیت های ما تا اینجا استفاده از dataset بود که باید شامل عکس هایی بسیار uniform باشد. حالا شرایط را بررسی میکنیم که تصاویر بزرگتر باشند و feature در هرجای تصویر (نه صرفاً در مرکز) قرار گرفته باشند.

در آنچه تاکنون مطالعه کردیم،یک dataset داشتیم که تصاویر مربوط به training و testing در آن جدا و مشخص بود.
\*در واقعیت اینگونه نیست و لازم است خودمان dataset را generate کنیم.
در اینجا چند مورد از API ها را بررسی میکنیم که در این امر ما را یاری خواهند کرد.

#### **Image Generator in TensorFlow.**

```ruby
from tensorflow.keras.preprocessing image import Image Data Generator.

train-datagen=Image Data Generator (rescale=1/255)*
*to normalize the data
train-generator=*train-datagen.flow-from-directory…….train-dir,
*باید directory آدرس داده شود و به sub-directory
target-size=(300,300)*,batch-size=128*,class-made=’binary’*
*همه‌ی تصاویر باید به سایز…. تبدیل شوند.
*بجای یک به یک 128 تا 128…..
*it is a binary class fitr
```

### صفحه هجدهم

Validation generator دقیقاً مثل train-generator است.

```ruby
validation-generator =test-datagen.flow-from-directory(validation-dir,
target-size=(300,300),
batch-size=32,
class-mode=’binary’)
```

در حقیقت کاری که ما باید بکنیم آن است که ترتیب زیر تصاویر را در یک directory,ذخیره کنیم و با استفاده از این API آن ها را load کنیم.

<!-- ![](../assets/images/posts/chapter-one/ch01-08.png) -->

خیلی جالب شد.وقتی که من به این ترتیب آدرس میدم و عمل میکنم(مثلاً آدرس training را میدهیم)،عکس های 1،2،3←lable
horses می خورند و کود میشود و عکس‌ها : Reza- Ahp-Al

### صفحه نوزدهم

در اینجا یک مثال human vs horses را بررسی میکنیم.از آنجا که تصاویر و feature ها نسبتاً بزرگتر از تمرینات قبلی هستند،3لایه convolution قبل از DNN در نظر گرفتیم.

```ruby
model=t.f.keras.models.sequential([t.f.keras.conv ZD(lb,(3,3),activation=’relu’,input-shape=(300,700,3)

t.f.keras.layers.Max Pool ZD(2,2),
t.f.keras.layers.Conv ZD (32,(3,3),activation=’relu’),
t.f.keras.layers.Max Pool ZD (2,2)
t.f.keras.layers.Con ZD(64,(3,3),activation=’relu’),
t.f.keras.layers.Max Pool ZD(2,2)
t.f.keras.layers.Flatten( ),
t.f.keras.layers.Dense(512,activation=’relu’)
t.f.keras.layers.Dense(1,activation=’sigmoid’)])

```

نکته:تصاویر به کار گرفته شده رنگی می باشند.به همین دلیل input-shape به صورت (300,700,3) می باشد

نکته:Sigmoid تابع بسیار مناسبی است برای binary cbssifi otb ← نکته‌اش این است که وقتی از sigmoid در خروجی استفاده میکنیم،باید یک neuron در نظر بگیریم. برخلاف softmax که نیاز به 2 neuron در خروجی دارد.
در حقیقت کاری که ما باید بکنیم آن است که ترتیب زیر تصاویر را در یک directory,ذخیره کنیم و با استفاده از این API آن ها را load کنیم.

```ruby
form tensorflow,keras.optimizers import RMSprop
model.compile(loss=’binary-crossentory’,optimizer=RMSprop(Ir=0.001),metrics=[‘acc’])
```

حالا-سراغ trainig میرویم. در اینجا fit کمی متفاوت است.

### صفحه بیستم

```ruby
History=model.fit-generator
Train generator,
Steps.per-epoch=8,
Epoch=15,
Validation-data=validation-generator,
Validation steps=8,
Verbose=2,
```

از آنجایی که به جای یک dataset از یک generator استفاده می کنیم بجای model.fit هم از model.fit-generator استفاده می کنیم
بعد از آنکه training انجام شد،باید predict کنیم و این کد این کار را برای ما انجام می دهد.

```ruby
Import numpy as np
From google colab import files
From keras . preprocessing import image
Uploaded=files.upload
For fn in uploaded keys
Path=content + fn
Img=image load-image(path,target-size (300,300))
X=image.img-to-array (img)
X=np.expand-dims(x,axis=0)
```
