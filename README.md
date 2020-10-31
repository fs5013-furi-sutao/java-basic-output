# Java の基本的な出力
Java の基本的な出力

## 最初に（要点）
Java で出力する（コンソール画面に文字を表示する）には System.out.println() を使う。

用途に合わせて他にも、改行のない System.out.print()、文字を当てはめて使う System.out.printf() がある。

***

## 標準出力とは
標準出力とは、コンピュータ上で実行されているプログラムが、特に何も指定されていない場合に標準的に利用するデータ出力先のこと。PC ではディスプレイ装置（画面）による利用者への文字表示が標準出力に設定されている。システム上では “stdout” （stdout：standard output）の略号で表される。

つまり、プログラムでは、特に何も指定しない場合、コンソール画面に文字が表示される。

## Java での出力方法
Javaでは、単純に標準出力（画面）に出力を送るために使うことができる。
```console
System.out.plinln();
```
さらっと System.out.println の内容を見ておく。
- System: クラス呼び出し
- out はすべてに公開（public）する静的フィールド（static）: 出力データを受け取る

ビギナーは分からないくても心配しないでね。後の内容、クラス（class）、アクセス修飾子（public）、静的メソッド（static）で詳しく学習する。

1行、文字列を表示してみる。
```java 
public class App {
    public static void main(String[] args) {
        System.out.println("I print out the one line.");
    }
}
```

