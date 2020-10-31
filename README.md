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

Javaで文字を標準出力するには、次のように書く。

``` console
System.out.println();
```

さらっと System.out.println の内容を見ておく。

* System: クラス呼び出し
* out はすべてに公開（public）する静的フィールド（static）: 出力データを受け取る

ビギナーは分からないくても心配しないでね。後の内容、クラス（class）、アクセス修飾子（public）、静的メソッド（static）で詳しく学習する。

1行、文字列を表示してみる。
```java 
public class App {

    public static void main(String[] args) {
        System.out.println("I print out the one line.");
    }

}
``` 

実行結果:
```console
I print out the one line.
```

ここでは、println() メソッドを使用して文字列を表示した。

## println（）、print（）、printf（）の違い

* print(): 引用符内の文字列を出力する
* println(): print() メソッドと同様に、引用符内に文字列し、カーソルを次の行の先頭に移動させる
* printf(): 書式を指定して文字列を出力する（C / C ++ プログラミングの printf と同じ）

println は print line （1行出力する）の略である。

## 例1: print() と println()

``` java
class Output {
    public static void main(String[] args) {
        System.out.print("1-print_");
        System.out.print("2-print_");

        System.out.println("1-println_");
        System.out.println("2-println_");
    }
}
```

実行結果:

``` console
1-print_2-print_
1-println_
2-println_
```

上記の例では print() と println() メソッドの動作を示している。printf() メソッドについては、別途 printf() メソッドの解説を見てほしい。

## 例2: リテラルと変数の出力

``` java
class Variables {
    public static void main(String[] args) { 	
        Double number = -10.6;
    	
        System.out.println(5);
        System.out.println(number);
    }
}
```

出力結果: 

``` console
5
-10.6
```

整数や変数などを表示するには、引用符を使用しない。
