# GymManager

**Факултетен номер:** 2301321082 
**Име на проекта:** Система за управление на фитнес зала  
**Тема:** Курсова работа по програмиране  
**Технологии:** ASP.NET MVC, Entity Framework, SQL Server (LocalDB)

## 📌 Описание

GymManager е уеб базирана система, предназначена за управление на фитнес зала. Чрез нея администратори могат да управляват потребители, треньори, добавки (supplements), повреди на уреди, оборудване и поръчки.

## 💻 Основни функции

- Регистрация и вход на потребители
- Роли: Администратор и потребител
- CRUD операции за:
  - Служители
  - Уреди
  - Повреди
  - Добавки
  - Поръчки
- Валидация на входните данни чрез `DataAnnotations`
- Сигурност чрез Identity логин система
- Свързана база от данни с EF Code First

## ⚙️ Инсталация и стартиране

1. Изтегли проекта.

2. Отвори `GymManager.sln` с Visual Studio

3. Увери се, че `Web.config` съдържа следната връзка:
```xml
<connectionStrings>
  <add name="DefaultConnection" 
       connectionString="Data Source=(LocalDB)\MSSQLLocalDB;Initial Catalog=GymDB;Integrated Security=True;" 
       providerName="System.Data.SqlClient" />
</connectionStrings>

4.Отвори Tools > NuGet Package Manager > Package Manager Console и изпълни:
Update-Database
5.Стартирай проекта с F5.
