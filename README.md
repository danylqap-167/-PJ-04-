Файл

conftest.py содержит весь необходимый код для отслеживания неудачных тестовых примеров и создания скриншота страницы на случай, если какой-либо тестовый пример завершится неудачей.


[base.py](https://github.com/danylqap-167/-PJ-04-/blob/main/base.py) содержит реализацию шаблона PageObject для Python.

pages/auth_page.py страница авторизации для работы с автотестами.

pages/registration_page.py страница регистрации для работы с автотестами.

pages/elements.py содержит вспомогательный класс для определения веб-элементов на веб-страницах.

autotests_rostelecom.py содержит тесты веб-интерфейса для Ростелекома (https://b2c.passport.rt.ru/)

Описание автотестов
test_start_page_is_correct

Тест-кейс N-01 Корректное отображение "Стандартной страницы авторизации"

test_location_of_page_blocks

Тест-кейс N-02 - Проверка элементов в левом и правом блоке страницы Тест не проходит(Bugs-02).Причина - расположение элементов на странице не соответсвует ожидаемым требованиям

test_phone_tab

Тест-кейс N-03 Проверка названия таб выбора "Номер" Тест не проходит(Bugs-03).Причина - Таб выбора 'Номер' не соответсвует ожидаемым требованиям

test_registration_page_and_continue_button

Тест-кейс N-04 Проверка название кнопки "Продолжить" в форме "Регестрация" Тест не проходит(Bugs-04). Причина - Кнопка должна иметь текст 'Продолжить'

test_registration_page_with_empty_name_field

Тест-кейс N-06 Регистрация пользователя с пустым полем "Имя", появления текста с подсказкой об ошибке

тест_регистрация_ с_an_incorrect_value_in_the_name_field

Тест-кейс N-07 Регистрация пользователя с некорректным значением в поле "Имя"(< 2 символов), появление текста с подскаской об ошибке

тест_регистрация_ с_an_incorrect_value_in_the_last_name_field

Тест-кейс N-08 Регестрация пользователя с некорректным значением в поле "Фамилия"(>30 символов), появление текста с подскаской об ошибке

тест_регистрация_of_an_already_registered_user

Тест-кейс N-09 Регистрация пользователя с уже зарегистрированным номером,отображается оповещающая форма

test_notification_form

Тест-кейс N-10 Проверка кнопки "х" - закрыть всплывающее окно оповещения Тест не проходит (Bugs-10). Причина - "Должна быть кнопка закрыть 'х'"

test_incorrect_password_during_registration

Тест-кейс N-11 Некорректный пароль при регестрации пользователя(< 8 символов), появления текста с подсказкой об ошибке

тест_авторизации_of_a_user_with_an_invalid_password

Тест-кейс N-12 Вход по неправильному паролю в форме "Авторизация" уже зарегистрированного пользователя, надпись "Забыл пароль" перекрашивается в оранжнвый цвет

test_instead_of_cyrillic_invalid_characters

Тест-кейс N-13 Регистрация пользователя в форме "Регистрации" в поле ввода "Фамилия" вместо кириллицы, недопустимые символы

test_password_and_password_confirmation_do_not_match

Тест-кейс N-14 Поле ввода "Пароль" и поле ввода "Подтверждение пароля" в форме "Регистрация" не совпадают

test_invalid_email_or_mobile_phone

Тест-кейс N-15 Не валидный email в поле ввода "Email или мобильный телефон"

test_authorisation_valid

Тест-кейс N-16 Тестирование аутентификации зарегестрированного пользователя
