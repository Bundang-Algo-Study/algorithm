# BOJ 15724λ² [μ£Όμ§μ](https://www.acmicpc.net/problem/15724)

## π νμ΄ νκΈ°
* 1μ°¨μ λ°°μ΄ λμ ν©λ§ νμ΄λ³΄κ³  2μ°¨μ λ°°μ΄ λμ ν©μ μ²μ νμ΄λ³΄λ κ² κ°μμ~

## π©βπ« λ¬Έμ  νμ΄
* λ°°μ΄μ΄ λ€μκ³Ό κ°μ΄ μ£Όμ΄μ§ λ 2μ°¨μ λ°°μ΄ λμ ν©μ dp λ°°μ΄μ λ£μ΅λλ€.
    * μλ ₯ λ°°μ΄
        |1|1|1|
        |---|---|---|
        |1|1|1|
        |1|1|1|
    * λμ ν© dp
        |1|2|3|
        |---|---|---|
        |2|4|6|
        |3|6|9|

* 2, 2, 3, 3 λ²μμ κ°μ κ΅¬νλΌκ³  νλ©΄,
    * dp[3][3]-(dp[3][1]+dp[1][3])+dp[1][1]
    * = 9 - (3 + 3) + 1
    * = 4 λ₯Ό μΆλ ₯νλ©΄ λ©λλ€.
 
