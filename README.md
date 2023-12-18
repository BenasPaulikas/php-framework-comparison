# php-framework-comparison

Welcome.
I've worked with Yii(1+2) framework for 10+ years.
Laravel only <1 year.
My personal opinion might be slightly biased. I will keep updating this.

These are major differences I've found out. I might be wrong here. Please create github issue if you don't agree with me.

## Feature Comparison

| Feature                  | Description | Yii2 | Laravel |
|--------------------------|-------------|------|---------|
| ActiveForm+ActiveField  | (allows easy form creation without using html tags like <form or <input) |  Y  |    N    |
| GridView                | (allows easy table creation without using html tags like <table) | Y   | N       |
| ActiveDataProvider | x | Y | ? |
| Time travel in tests     | x | N   | Y       |
| Auto generated default URL rules for controller | X | Y | ? |
| x | x | yii *migrate*/down yii *migrate* | artisan make:*migration* > artisan *migrate*
| Out of the box scheduling | x | N https://github.com/omnilight/yii2-scheduling | Y
| AND in query | x | User::find()->where()->andWhere() | User::query()->where()->where()
| TODO audit package |X | ? | Y |
| TODO auto urlManager/routes | X | Y | ?|
| Rules found in | x | Model rules+scenarios | Form |
| file cache expiration | x | y (gc kicks in at some small chance?) | n? |
| debug\profiler |x | y(not only shows query but location in code) | https://github.com/jkocik/laravel-profiler?|
| pusher | x | ? | y |
| html components | x | Widget class | blade components
| x | TODO explain which one is more bulletproof | Yii::$app->urlManager->getAbsoluteUrl() | url()->current()
