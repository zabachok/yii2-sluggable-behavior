Sluggble behavior
=================
Поведение для транслитерации кирилицы в латиницу.

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist zabachok/yii2-sluggable-behavior "*"
```

or add

```
"zabachok/yii2-sluggable-behavior": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

Behavior for transliterate russian text to latin.

Использовать так же как и оригинальное поведение. Класс унаследован от \yii\behaviors\SluggableBehavior
просто переопределен метод generateSlug

```php
use zabachok\behaviors\SluggableBehavior;

public function behaviors()
{
	 return [
		 [
			 'class' => SluggableBehavior::className(),
			 'attribute' => 'title',
			 // 'slugAttribute' => 'slug',
		 ],
	 ];
}
```