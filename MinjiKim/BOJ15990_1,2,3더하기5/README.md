# BOJ 15990λ² [1, 2, 3 λνκΈ° 5](https://www.acmicpc.net/problem/15990)

## π νμ΄ νκΈ°
* μμ΄λ‘ νμλ€κ°,, μκ°μ΄κ³ΌλΌμ dp λ°©λ²μ μ°Ύμλ΄€μ΅λλ€.

## π©βπ« λ¬Έμ  νμ΄
* dpλ λ°©λ²μ μκ°νλ κ² μ΄λ €μ΄ κ² κ°μ΅λλ€.
* ```dp[λ§λ€κ³  μΆμ κ°][κ°μ₯ λ§μ§λ§μ μ€λ μ]``` 2μ°¨μ λ°°μ΄μ λ§λ­λλ€.
* dp[y][1]=dp[y-1][1λ‘ λλλ μ], dp[y-1][2λ‘ λλλ μμ ] 1μ λνλ©΄ λκΈ° λλ¬Έμ, ``` dp[y][1] = (dp[y - 1][2] + dp[y - 1][3]) % 1_000_000_009;``` λ₯Ό λ£μ΅λλ€.
* λ§μ°¬κ°μ§λ‘ dp[y][2], dp[y][3]μ μ±μλλ€.