![simplinnovation](https://1.bp.blogspot.com/-wStk0VZDfMk/YCC0GIRPrDI/AAAAAAAAAGc/1yj7IOUedvoeO1CuCxq7ETLW0FqXni6mwCLcBGAsYHQ/s320/logotext.png)

# __Circuiti*k*Z__

[![Video](https://img.youtube.com/vi/EXUcCZnR1bg/0.jpg)](https://www.youtube.com/watch?v=EXUcCZnR1bg)

__Circuiti*k*Z__ merupakan free package untuk menyisipkan gambar skema/diagram rangkaian komponen elektronika di dokumen LaTeX. Tutorial kali ini membahas step-by-step bagaimana cara menggambarkan skema rangkaian elektronika di dokumen LaTeX menggunakan __MiKTeX__, __Visual Studio Code__ dan package __Circuiti*k*Z__. Jika Anda belum familiar dengan LaTeX, ada baiknya simak tutorial dasar LaTeX menggunakan MiKTeX & VS code berdurasi 2 jam berikut (_klik gambar berikut_).

[![Video](https://img.youtube.com/vi/S_D16cfhxtE/0.jpg)](https://www.youtube.com/watch?v=S_D16cfhxtE)

#

## __A. Instalasi__

1. Open __MiKTeX Console__, pada _Operation Mode_ pilih salah satu opsi role: sebagai __admin__ (_Switch to MiKTeX administrator mode_) atau __user__ (_Stay in MiKTeX user mode_).

2. Masuk menu _Packages_ lalu ketik _circuitikz_ di text input, kemudian install dengan klik icon plus (`+`).

#

## __B. Contoh Penggunaan__

- LaTeX script:

    ```latex
    \documentclass{article}
    \usepackage{circuitikz}

    \begin{document}
        \section{Symbol}
        \subsection{Resistor}
        \begin{enumerate}
            \item Basic Resistor
            
            \begin{circuitikz}[american]
                \draw (0,0) to[resistor] (2,0);
                \draw (2.5,0) to[R] (4.5,0);
                \draw (5,0) to[R, l=$R_1$] (7,0);
                \draw (7.5,0) to[R, a^=$5\Omega$] (9.5,0);
            \end{circuitikz}

            \vspace{0.3in}
            
            \begin{circuitikz}[european]
                \draw (0,0) to[resistor] (2,0);
                \draw (2.5,0) to[R] (4.5,0);
                \draw (5,0) to[R, a=$100\Omega$] (7,0);
                \draw (7.5,0) to[R=$10\Omega$] (9.5,0);
            \end{circuitikz}

            \vspace{0.3in}

            \begin{circuitikz}
                \draw (0,0) to[R=$133\Omega$, i=$10mA$, v=$3mV$] (3,0);
            \end{circuitikz}
            \begin{circuitikz}[european]
                \draw (3.5,0) to[R=$133\Omega$, i=$10mA$, v=$3mV$] (6.5,0);
            \end{circuitikz}
        \end{enumerate}
    \end{document}
    ```

- Output:

    ![circuitikz output](https://1.bp.blogspot.com/-rdzhjQZl_Iw/YC3y2qlEOrI/AAAAAAAAAG0/Cc2ktM4r8hoj3BjtpsJoaCMdwY9FcuF6gCLcBGAsYHQ/s320/Anotasi%2B2021-02-18%2B115218.png)

#

#### 🍔 Lintang Wisesa

<br>

<a href="mailto: lintangwisesa@ymail.com">
  <img align="left" style="margin-right:10px" alt="lintang ymail" width="22px" src="https://camo.githubusercontent.com/b6e5ff081d7552ec05656de193794847e14d47ad/68747470733a2f2f732e79696d672e636f6d2f63762f61706976322f6d79632f6d61696c2f4d61696c5f694f535f6170705f69636f6e2e706e67" />
</a>

<a href="https://web.facebook.com/lintangbagus/">
  <img align="left" style="margin-right:10px" alt="lintang facebook" width="22px" src="https://camo.githubusercontent.com/a461898d72dd9f4c8c526dfcca9dfdc8a8c69605/68747470733a2f2f75706c6f61642e77696b696d656469612e6f72672f77696b6970656469612f636f6d6d6f6e732f7468756d622f352f35312f46616365626f6f6b5f665f6c6f676f5f253238323031392532392e7376672f3130323470782d46616365626f6f6b5f665f6c6f676f5f253238323031392532392e7376672e706e67" />
</a>

<a href="https://twitter.com/Lintang_Wisesa">
  <img style="margin-right:10px" align="left" alt="lintang twitter" width="24px" src="https://camo.githubusercontent.com/b6943877f3d8a1269974b9f820388403ee2b1978/68747470733a2f2f332e62702e626c6f6773706f742e636f6d2f2d4e786f754d6d7a32624f592f54385f61633937636573492f41414141414141414767302f65337659315f62646e62452f73313630302f547769747465722b6c6f676f2b323031322e706e67" />
</a>

<a href="https://www.youtube.com/user/lintangbagus">
  <img style="margin-right:10px" align="left" alt="lintang youtube" width="29px" src="https://www.pinclipart.com/picdir/big/55-557137_a-quiet-drifter-takes-a-janitorial-job-at.png" />
</a>

<a href="https://www.linkedin.com/in/lintangwisesa/">
  <img style="margin-right:10px" align="left" alt="lintang linkedin" width="24px" src="https://camo.githubusercontent.com/0d70d8c72e2f45755511d6799489dc49d0e325f0/68747470733a2f2f692e70696e696d672e636f6d2f6f726967696e616c732f63652f30392f33632f63653039336337323134616433353762623636356366643266363661386236622e706e67" />
</a>

<a href="https://github.com/LintangWisesa">
  <img style="margin-right:10px" align="left" alt="lintang github" width="23px" src="https://camo.githubusercontent.com/11406e7ae7d4716fcc586cddf450451576d71bef/68747470733a2f2f696d6167652e666c617469636f6e2e636f6d2f69636f6e732f7376672f32352f32353233312e737667" />
</a>

<a href="https://www.hackster.io/lintangwisesa">
  <img style="margin-right:10px" align="left" alt="lintang hackster" width="23px" src="https://user-images.githubusercontent.com/10383395/49821324-358fa080-fda0-11e8-8b00-def2a67fc598.png" />
</a>

<a href="https://lintangwisesa.github.io/me/">
  <img style="margin-right:10px" align="left" alt="lintang bio" width="24px" src="https://avatars2.githubusercontent.com/u/30064213?s=460&u=6640a1c3d5c1892283e1c273006755de8d32fa59&v=4" />
</a>