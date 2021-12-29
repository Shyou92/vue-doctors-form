<template>
  <form class="form">
    <fieldset class="form__container">
      <div class="form__itemContainer">
        <label class="form__label" for="surname">Фамилия*</label>
        <input class="form__item" type="text" id="surname" />
        <span class="form__error"
          >Поле Фамилия обязательное для заполнения
        </span>
        <span class="form__error"
          >Поле Фамилия должно иметь текстовый формат
        </span>
        <span class="form__error"
          >Поле Фамилия должно иметь больше, чем 2 символа
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="firstname">Имя*</label>
        <input class="form__item" type="text" id="firstname" />
        <span class="form__error">Поле Имя обязательное для заполнения </span>
        <span class="form__error">Поле Имя должно иметь текстовый формат </span>
        <span class="form__error"
          >Поле Имя должно иметь больше, чем 2 символа
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="lastname">Отчество</label>
        <input class="form__item" type="text" id="lastname" />
        <span class="form__error"
          >Поле Отчество должно иметь текстовый формат
        </span>
        <span class="form__error"
          >Поле Отчество должно быть длиной больше, чем 2 символа
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="date-of-birth">Дата Рождения*</label>
        <input class="form__item" type="date" id="dateOfBirth" />
        <span class="form__error"
          >Поле Дата Рождения обязательно для заполнения
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="phone">Номер телефона*</label>
        <input class="form__item" type="tel" id="phone" />
        <span class="form__error"
          >Поле Номер Телефона обязательно для заполнения
        </span>
        <span class="form__error"
          >Поле Номер Телефона должно состоять только из цифр
        </span>
        <span class="form__error"
          >Поле Номер Телефона должно иметь 2 цифр
        </span>
        <span class="form__error"
          >Поле Номер Телефона должно иметь 2 цифр
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="gender">Пол</label>
        <input class="form__item" type="text" id="gender" />
        <span class="form__error">Поле Пол должно иметь текстовый формат </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="clients">Группа клиентов*</label>
        <select
          class="form__select form__selectMultiple"
          size="3"
          multiple
          id="clients"
        >
          <option value="vip" class="form__selectOption">VIP</option>
          <option value="problem" class="form__selectOption">Проблемные</option>
          <option value="oms" class="form__selectOption">ОМС</option>
        </select>
        <span class="form__error form__errorSelectMultiple"
          >Выберите обязательно хотя бы одно поле
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="doctor">Лечащий врач</label>
        <select class="form__item form__select" id="doctor">
          <option value="ivanov">Иванов</option>
          <option value="zakharova">Захаров</option>
          <option value="chernysheva">Чернышева</option>
        </select>
      </div>
      <div class="form__itemContainer form__itemCheckbox">
        <label class="form__label form__labelCheck" for="sms"
          >Не отправлять СМС</label
        >
        <input class="form__item form__itemSms" type="checkbox" id="sms" />
      </div>
    </fieldset>
    <fieldset class="form__container">
      <h3 class="form__item-header">Адрес:</h3>
      <div class="form__itemContainer">
        <label class="form__label" for="postnumber">Индекс</label>
        <input class="form__item" type="text" id="postnumber" />
        <span class="form__error"
          >Поле Индекс должно состоять только из цифр
        </span>
        <span class="form__error"
          >Поле Индекс должно быть длиной в 2 символов
        </span>
        <span class="form__error"
          >Поле Индекс должно быть длиной в 2 символов
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="country">Страна</label>
        <input class="form__item" type="text" id="country" />
        <span class="form__error"
          >Поле Страна должно иметь текстовый формат
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="region">Область</label>
        <input class="form__item" type="text" id="region" />
        <span class="form__error"
          >Поле Область должно иметь текстовый формат
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="city">Город*</label>
        <input class="form__item" type="text" id="city" />
        <span class="form__error">Поле Город обязательно для заполнения </span>
        <span class="form__error"
          >Поле Город должно иметь хотя бы 1 букву
        </span>
        <span class="form__error"
          >Поле Город должно иметь текстовый формат
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="street">Улица</label>
        <input class="form__item" type="text" id="street" />
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="house-number">Дом</label>
        <input class="form__item" type="text" id="house-number" />
        <span class="form__error">Поле Дом должно иметь цифровой формат </span>
      </div>
    </fieldset>
    <fieldset class="form__container">
      <h3 class="form__item-header">Паспорт:</h3>
      <div class="form__itemContainer">
        <label class="form__label" for="document">Тип документа*</label>
        <select class="form__item form__select" id="document">
          <option value="passport">Паспорт</option>
          <option value="certificate-of-birth">Свидетельство о рождении</option>
          <option value="driver-license">Вод. удостоверение</option>
        </select>
        <span class="form__error">Выберите тип документа</span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="docs-series">Серия</label>
        <input class="form__item" type="text" id="docs-series" />
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="docs-number">Номер</label>
        <input class="form__item" type="text" id="docs-number" />
        <span class="form__error"
          >Поле Номер Документа должно состоять из цифр
        </span>
        <span class="form__error"
          >Поле Номер Документа должно состоять 2 цифр
        </span>
        <span class="form__error"
          >Поле Номер Документа должно состоять 2 цифр
        </span>
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="docs-organization">Кем выдан</label>
        <input class="form__item" type="text" id="docs-organization" />
      </div>
      <div class="form__itemContainer">
        <label class="form__label" for="date-of-issue">Дата выдачи*</label>
        <input class="form__item" type="date" id="date-of-issue" />
        <span class="form__error"
          >Поле Дата Выдачи обязательно для заполнения</span
        >
      </div>
    </fieldset>
    <button class="form__submit">Отправить</button>
    <span class="form__warning">* Поле, обязательное для заполнения.</span>
  </form>
</template>

<script>
export default {};
</script>

<style></style>
