### HTTP - Hypertext transfer protocol

1. What is CORS? How does it work?

2. Explain the purpose of each of the HTTP request types when used with a RESTful web service.

3. What is a “MIME type”, what does it consist of, and what is it used for? Provide an example?

### OOP (Object Oriented Programming)

1. What are the differences between abstract and interface?

2. What is polymorphism in OOP? Give an example.

3. What is MVC pattern? What other patterns do you know and when do you use them?

### PHP (Hypertext Preprocessor)

1. What are the differences between === and ==?

2. Assume you have a table Posts and a table Categories, How would you build the news pages using the MVC pattern?

3. What are the steps involved when you run a find query from the controller or model in the MVC framework that you are mostly familiar with? (Any framework is fine)

4. Please write the differences between "many to many" and  "many to one"?

5. What is the output with the following code? Please explain your answer.

```php
<?php

class Vehicle
{
    public function getMake()
    {
        return __CLASS__;
    }
}

class Mercedes extends Vehicle
{
}

$car = new Mercedes();
echo $car->getMake();
```

6. What are the errors of this code? What is intended to print?

```php
class Mercedes
{
    public function __construct($flag = true)
    {
        $this->latest = $flag;
    }

    public static function getBuiltYear()
    {
        $year = new \DateTime('now');
        if (!$this->latest()) {
            $year->modify('-1 year');
        }

        return $year->format('Y');
    }
}
```
