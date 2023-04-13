# Lab-7_202001155
# IT314 Lab 7
## NAME: Harsh Ramoliya
## ID: 202001155

### Section A

### Equivalence Class
Day:
|ID| class | validity |
|--|-------|----------|
|El| dd<1 |Invalid |
|E2 |1<=dd<=28| Valid|
|E3 |dd=31 |Valid |
|E4| dd=29 |Valid |
|ES |dd=30| Valid |
|E6| dd > 31| Invalid |

Month:

|ID| class | validity |
|--|-------|----------|
|E7| mm<1 |Invalid |
|E8 |mm = 1,3,5,7,8,10,12(months with 31 days) | Valid|
|E9 |mm = 4,6,9,11(months with 30 days) |Valid |
|E10|mm = 2(month with either 28 or 29 days) |Valid |
|E11 |mm > 12| Invalid |

Year:
|ID| class | validity |
|--|-------|----------|
|E12| yy<1900 |Invalid |
|E13 | leap year 1900<=yy<=2015 | Valid|
|E14 |non leap year 1900<=yy<=2015  |Valid |
|E15 |yy > 2015 |Invalid |

Equivalence Partitioning Test Cases:

<table>
  <tr>
    <th>Tester Action and Input Data</th>
    <th>Expected Outcome</th>
  </tr>
  <tr>
    <td>Valid input: day=1, month=1, year=1900</td>
    <td>Invalid date</td>
  </tr>
  <tr>
    <td>Valid input: day=31, month=12, year=2015</td>
    <td>Previous date</td>
  </tr>
  <tr>
    <td>Invalid input: day=0, month=6, year=2000</td>
    <td>An error message</td>
  </tr>
  <tr>
    <td>Invalid input: day=32, month=6, year=2000</td>
    <td>An error message</td>
  </tr>
  <tr>
    <td>Invalid input: day=29, month=2, year=2001</td>
    <td>An error message</td>
  </tr>
</table>

Boundary Value Analysis Test Cases:

<table>
  <tr>
    <th>Tester Action and Input Data</th>
    <th>Expected Outcome</th>
  </tr>
  <tr>
    <td>Valid input: day=1, month=1, year=1900</td>
    <td>Invalid date</td>
  </tr>
  <tr>
    <td>Valid input: day=31, month=12, year=2015</td>
    <td>Previous date</td>
  </tr>
  <tr>
    <td>Invalid input: day=0, month=6, year=2000</td>
    <td>An error message</td>
  </tr>
  <tr>
    <td>Invalid input: day=32, month=6, year=2000</td>
    <td>An error message</td>
  </tr>
  <tr>
    <td>Invalid input: day=29, month=2, year=2000</td>
    <td>An error message</td>
  </tr>
  <tr>
    <td>Valid input: day=1, month=6, year=2000</td>
    <td>Previous date</td>
  </tr>
  <tr>
    <td>Valid input: day=31, month=5, year=2000</td>
    <td>Previous date</td>
  </tr>
  <tr>
    <td>Valid input: day=15, month=6, year=2000</td>
    <td>Previous date</td>
  </tr>
  <tr>
    <td>Invalid input: day=31, month=4, year=2000</td>
    <td>An error message</td>
  </tr>
</table>
</br>
