# Danila Kostenko
---
### Junior .NET Developer
---
### Contact
+ **Location:** Russia, Saint-Petersburg
+ **Email:** <danil.kostenko@outlook.com>
+ **Phone:** +7-928-954-09-38
+ **Telegram:** [@Kostenko_Danila](https://t.me/Kostenko_Danila)

### Summary

I am 22 years old. I am a second-year master's student at LETI. At the moment I am doing an internship at EPAM in the direction of .NET development. I have experience working in companies in positions .NET-developer and programmer-analyst. My goal is to grow in .NET and JS development.

### Skills
+ .NET Core 2.2, 3.1, 5
+ C#
+ RabbitMQ
+ Entity Framework, Dapper
+ MS SQL Server, T-SQL, Elasticsearch
+ JS (ES6+) 
+ HTML&CSS
+ GIT

### Experience

+ [INOSTUDIO](https://inostudio.com/en/) (December 2019 - August 2020):
    + **Position:** Junior .NET Developer 
    + **Responsibilities:**  as a .NET developer, I am responsible for implementing the business logic part of new functionality, fixing bugs, create new store procedures from scratch using T-SQL, writing unit tests.
+ [Lasmart](https://lasmart.ru/) (October 2020 - April 2021): 
    + **Position:** Programmer-analyst (October 2020 - April 2021)
    + **Responsibilities:** Setting up ETL processes, writing stored procedures in T-SQL, creating reports for business analysts in MS Report Service, communicating with customers and drafting technical specifications.
+ [EPAM](https://www.epam-group.ru/) (August 2021 - Present)
    + **Position**: trainee (.NET)
    + **Responsibilities:**: Performing training tasks using .NET 5, React, SQL Server, Azure services. Creating an application on a microservice architecture, writing unit tests.

### Education

+ **Bachelor, Taganrog (2016-2020):** 
    + Southern Federal University (SFedU)
    + Department of Information Security
+ **Master, Saint-Petersburg (2020-2022):**
    + St. Petersburg Electrotechnical University (LETI)
    + Department of Computer-aided Design Systems

### Languages

+ **Russian** - native speaker
+ **English** - A2+ (EPAM English assesment August 2021)
+ **Ukrainian** - native speaker

### Code examples

```cs
public static class EnumerableExtensions
{
    /// <summary>
    /// Cartesian product of enumerated elements
    /// </summary>
    public static IEnumerable<IEnumerable<T>> CartesianProduct<T>(
        this IEnumerable<IEnumerable<T>> source) =>
        source.Aggregate(
            (IEnumerable<IEnumerable<T>>)new[] { Enumerable.Empty<T>() },
            (acc, src) => src.SelectMany(x => acc.Select(a => a.Concat(new[] { x }))));
}
```