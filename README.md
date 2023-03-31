### Hexlet tests and linter status:
[![Actions Status](https://github.com/tamara250/data-analytics-project-92/workflows/hexlet-check/badge.svg)](https://github.com/tamara250/data-analytics-project-92/actions) SELECT FIO_saler,
       SUM(price) AS summa
FROM   sales
WHERE  date_sale > '2015-12-23'
AND    date_sale < '2015-12-31'
GROUP  BY FIO_saler
HAVING SUM(price) > (SELECT SUM(price) FROM sales WHERE FIO_saler='Иванов Иван Иванович');
