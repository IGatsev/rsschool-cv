# CV - Гацев И.

### Имя и фамилия
+ Гацев Игорь

### Контакты для связи
+ +996 555 775377

### Цель
+ пройти курс Front End, вспомнить базу и получить знания для Full Stack разработчика

### Языки и фреймворки
+ Java, С#, Spring Boot, Andtoid, HTML, JS, CSS


### Примеры кода
```
function sendSms(){
        var phone = $('#signerPhone').val();
        if (phone == ''){
            alert('Введите телефон');
            return;
        }
        $.ajax({
            url: "signers/sendsms",
            type: "POST",
            datatype: "json",
            contentType: "application/json",
            data: JSON.stringify({
                signerId: $('#signerId').val(),
                signerPhone: '+996' + phone,
            }),
            success: function(data, textStatus, jqXHR) {
                if (data.success) {
                    showSuccessMsg('смс выслано');
                    $('#butSave').removeAttr("disabled");
                }else{
                    showFailureMsg(data.message);
                }
            },
            error: function(jqXHR, textStatus, errorThrown) {
                showFailureMsg("StatusText = " + textStatus + "\n" + "StatusCode = " + jqXHR.status + "\n" + "errorThrown = " + errorThrown.message);
            }
        });

    }
```


### Опыт работы.
+ Middle Dev:
Разработка платежных API, разработка мобильного приложения

### Образование (включая пройденные курсы и тренинги)
+ Неполное высшее КРСУ

### Английский язык
+ Уровень B2, был опыт работы с англоговорящими.