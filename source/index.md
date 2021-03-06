<h1 class="title">《Deepin 开发指南》<a href="https://github.com/loliMay/deepin-develop-guide"><img src="https://img.shields.io/github/stars/loliMay/deepin-develop-guide.svg?style=social"/></h1><p class="intro">一直以来都有个想法，去为 deepin 写一些文档，借此方便后来的开发者，帮助他们尽快地投入到 deepin 应用软件的开发中。于是出现了这一系列教程，这份《Deepin 开发指南》就是为 deepin developer 量身打造的入门教程，从开发环境的搭建与配置、编写一个完整项目到可执行文件的打包，涵盖了项目开发的整个流程，教程的最后还有 deepin tool kit 的完整 API 手册，供开发者查阅。由于作者本人才疏学浅，错误难免，欢迎在评论区中指正或者给作者提 [PR](https://github.com/loliMay/deepin-develop-guide/pulls)。</p><p class="intro">你可以通过以下方式支持作者的工作：<p class="intro indent">方式一 [star](https://github.com/loliMay/deepin-develop-guide) 这个项目(右上角 star)，你的 star 是作者坚持写下去的源动力</p><p class="intro indent">方式二 [参与写作&校对](https://github.com/loliMay/deepin-develop-guide#user-content-%E5%8F%82%E4%B8%8E%E5%86%99%E4%BD%9C%E6%A0%A1%E5%AF%B9)</p><p class="intro">最后，希望这份教程能够对你有所帮助，Have fun！</p><div class="button-box"><a href="intro/start.html"><div class="homepage-button">起步</div></a><a id="forum-button" href="https://bbs.deepin.org/forum.php?mod=viewthread&tid=167205" target="_blank"><div class="icon-button"><svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" width="128px" viewBox="0 0 128 128" enable-background="new 0 0 128 128" xml:space="preserve">  <image id="image0" x="0" y="0"
    xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABGdBTUEAALGPC/xhBQAAACBjSFJN
AAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QA/wD/AP+gvaeTAAAg
lElEQVR42u1deXRTx7n/jXZLsuQd7whssMGUfQ0hkBACBBJoCIQAAZIWSpbXHPJoXtOkD2gfaV9K
m9c0bcgOKWlooQESwpYFnABhLRgMtrENxja28a7NlmXpzvtD2JZ0r6Qr6V4ZmvzOmYPRne3OfPPN
t81c4Ht8j+/x3QXp7Q4Ijb6XO1SEIBcgOQCyQUg2gHQAyQC0AAwBqqgAYAFQB6AalCkDUAaghDIo
vpajtPX2OwqJ254A+pZ0GEAwmRAyHsB4AEMAyERqzgGgEMBxSulxUORfy1FW9PYYhIPbjgD6Ftlk
IJgMQuYSghkAsnu5S2WUYj8o3QWK/GuDVI7eHqNgcNsQQN8i22QiIUsAzAWQ0Nv98YFGALsoQ7dd
G6T6src7wwe3NAH0vdieDAlZRghWIfDezQL1+n+ilEAp6fnXHU4K1DooOhigwUl5t+EHFaB0Exhs
uZYXVddLQxgQtyQB9L3YngcJWQNgIQBVuPWNVxNszVBAFsTbVndS1HZSXOukKOmgKLdTnG1n0BI8
g7cB2AZKN17Li7oYuVHkh1uKAPoWtg2DhKyDi80LAjUhOJilQLpcmFet6qQ4187giJXBUSuDantQ
3GIXpXRd5RB1gZDjFg5uCQLIPG81EIlkLQiWd/8oCBcG1qfIsCxOLKUAKLExOGhmsNfkRJGNd6c3
U4ZZXzlUUyFax3iiVwkgs8CqAsGLhJA1EIDVe+MHUQQ7+yshI5F5zRIbgx2tTuxodfDZKmyU0o2g
2FA5TNNrtoVeI4DMAut0QsgmhCDc8cX2/gqM0Ugj+l5n25xYec2OBgfAk41VUEpXVQ7THohoR28i
4gSQedYSAwl5FXBj9yLgfr0Ub/RVRvTd9rY68J/VdrQxIRXfDIaurhyhbY1knyNKAJlnzRNBJFsh
+Kr3XGlSAnyVEwWDt64nIjY3duJX1+1whldNBRi6pHJk9NFI9TtiI5TxL/NagBwGpQZQCmETPNIP
Y2QRnfxX6+xYW22H06sfISQDCDnsGqvIQHQOkHHapCUSsh3AjEi9VP5gdUQIwEEpNly3472GTuEr
p9hPGTq/aozOIuY7iEoAGadMWURC9gDIFbMdd9ynl+HtLMEVChYclOKZqzbsa/XB9IVRY4spw8yu
GqsvF+s9RCOAjFOmiYRgB1xu2IhhR44aY7TiSv4dDMWzV23YF0DXE8iUUQdKH64aqxdFLhCFADJO
GmeBkG1w+d/DB8+RHKyWYH+eRoxX6obVSbH0cjtOWcIU94KDBZQurBqn/0zoigXfKDOOt84DsAsM
1YKhECTxFAaXJMpFnQWrk2JpSRtOmR0CC7EBkxbArnTX2AoKQTlA+ret84hr5Ytne/UBtRQ4MyIa
Gqk4u1pzJ4MVpe04ZRZr5fNicw5KsbB6Qsw/hWpVMA6QfqxlFnF5vWQRXh0Apbg/Viba5NfbGcy7
ZMUpk5grH3ySjADb0o+1zBLq3QQZsfQjLROJhOyHUHt+CPhwsAaT9MIznno7g0cuWlDeHpp5TyRY
QDGj6s7YsAXDsAkg/evmLEjIEURY2ndHipLg5Gi94PXW2xksKLzlJr8LdRJK76ycFBeWihjWFpCe
36QFIXtAkezJqiLL/u+LFV74q7czWHDBgvI2Z8Tfh2dKZoA9GflNYXHd8HgmIdtBacSMPL4wPV5Y
Aqi3M1hw3izsyhfIKOCFXAqyHcDMUCsIeQtIP9y0FgTrRHmtIKCTERRMiBHM519vZ7CgwOxa+QIi
UUlgUEmRrpIgRSlBnFyCODlBslLiM1RNLSGIl7uYdLKS4NHzZhxv5TQ+raueEr8+lH6FNGpphxon
EkIOoxfUPW88mKjAnwcLI3vW2xksOGdCeYj+XACIlROM1MmQo5EiTytDlloCQ5RUEA3F5KB48F9G
rv45COiUqrsTghYKg+5V2pcNMURCLsB12iZ8hMkafz9IiwXJ4fv96+0MFpw1Bb3yExUEU+IVGB8j
w1i9HIYocc3QZW1OzDptRBs7crkClI6onprYGkx9Iaxg8ipl2JP/mxwNXiixivryXJgQEz4Tqrcz
mP8v/pOfrJRgQYoS0xMVGBYdWSaYrZbilRwNnr5o9n5kAPAqgMeDqS8oDpD2ef10ELLf+/cl6Sr8
NkeLycdbUG6NnI08SyNF/vjYsOqo72Aw/19GXpM/PlaOVZlRmBIvj1icoS/8vNiCrdfZoYSE0hnV
05J4h5fxVgNTD9arALLJ2zqVpZbil9kuB8xInSzcgIig0lh9eNK/a/JbUW71b+GbmqDAZ2NisGOk
HvcmKHp98gHgl9kaZEVJWH2lwKa0gzd4+8ODsAPQF72jeaSgeHWwtlvAmRAjj6guPCYMy5/VQbH8
nBHlFqdPAhujl+Mfo/TYMkyHYbpel3c9oJERvJoXDSlY/TaA4kW+9fAigNT9dQZCyRrvAVqeEYWR
bqtwQqycYyDFI4ChIU6Kg1I8dcGI88ZOznqTFRL8+QfR2DkmBnfEKnpjfnlhpF6O5RlR7HcA1qTt
rzPwqYMnByBrQanKY5CUBM9nefreM6KkSFeRoJwcoc6/WkKQqw2NAH5fZsUX9XZWnVIATxnUOHpn
HOYkq1Brc+If19uxu5a917582YK/VbfD2Nm7ZuLnszRIVkhAGbgnFaVkLZ/yAQkgdW/dMFC6nFIK
9/TCAC00HBaMCbEKeOf1l0KlgMHRoalb+2/Y8Fq5lVXfSJ0Me8fH4RcDtThj7MTi0y0YfbgRqy+Y
cKixg6OeDvys0IQ/lrs0nxpbRANEuqGREbwwUMs1RstTP6sdFqg8Hw6wznvVjtTLMS+VW86YkqCI
iACYF4L6VdXuxOrzJoBBd5JS4PlsLXaOj0WsgmDZ6RbMP96Cw/X27jwqDqEvSSEBGOCLehdxfFxj
Q7G5d64GmJeqcm2H3uMEsi5QWb8EkLKnNg+UzvWmrhcG+ra8TUlQ3BRMBN7zvaKEsjXBE8DqAiNM
dqa7ToNagk/viMOz2RrICMFLF0344kYHq+1EBXuYEhWura7c7ECzncFjGVFYdroFJ5vtEZ38Lvwy
N5pr3OamflqTFzIBEAqW4DchToE74n0LRnq5BCP1Mo9VJkjy6kd2kEe+3q9ow7eN9u7y9yYpcfDO
BAxzE2JNdh8yCweUhHQ/P9lsh14uwQqDGotP9g4R3BGvwIQ4Di0MWOOvnE8CSNl9PRmULvReec8N
CGx3vzdJKboKmBUEB6hpd+LlIlPPilYSvDUyhiXD1LZz2wPiOI6Wp6p6dPDzra5zAY9lqqGRAotP
NONkU+SJ4LkBWi4CXpiy+7rPWA1/HGAZpVC5j8VQvdzv6u/CrBSVqPMvBZAahM395SIzrJ20u/z4
OAWUHM6ZmjYnt8bBkVdK0C3IFhpdBKCUEjydpYW1k8Gi400oNolwYMQP7khQYnC0zFvQVoFima8y
vgmAYpX3SKzK4hdy3U8jQ55OJhoFJKv4268KjZ34uKrNo7xKwp7QqjYHOpzc7WWoOYjNbZUVtPSs
9sf6qpGokKDNQfHIsSbUtEdWO3iGiwsAq3zl5xzJ5I+rp960KHVXkqiUYHoy/xM3s1JUQUr2/Akg
I4jV//tiE0d59mtf9GEUAqVIUXG11/O8webstgeopASPGTTdvy8+1gSrI3K2gunJKpfQ6vkOhuSP
qyZz5eckAAIs9B6EeelRUAXh056TFhXUpAZDLIk8z/0VGjtxoMbGKh8rZ5c/02z32V5KlH8OAApU
WHpUwKUGNZTE9XuJqRPPnG4Ra75ZUEkJ5qVHsYRoQskSrvyskUjeUSXjUv0WZKqD6kg/rQxD9eL4
BvjuAJsumznL58WwnUjfNnRw5k2PkvomfLd8V90IIEklxYyUngVwoKYdfyoxRYYCACzoq+Z6l7nJ
2ytZkjN7KCmdDIoED6OLTo5cXfCet3mZUUFuA/wSN0v2hNHO4LPqdlZZJSEYFuMpyDZ1OFHQZPc2
p4IyQI4PgxOlnvmqvdzgjxrUHs9fKTR5yApiIlcnx2C93JsGEgCwtgEOAsBcb3PtrLSokDryUIYa
EgDBmIb5JD470Z7rbbA5GFCGeqQpfZSsFX24zgaHjyNo2b78DV756m2eVsC7klRIcXPXOhiKp080
wSbMHYQBMTtNxbXNzuVDADO8V82M1NAIIF4pxYzUm8Kg0EahANhd2cbJPWZzEPOOa20+uc0oH2pv
bbunG7mpgy3ozUlXe+QpNznwv4XGcOaVN2akurfdTQSsOxo8CKDPtgoDQLO7CzCuPTA3jMCLxQZN
UAc8eQuMfmB1MDh2w8YqF6cgmJXuKcvUtDnwTV27z7aG+XAH2xye+Wrb2H6AGRyC8NslJhQbxd8K
cvVypKslPePlStl9Pqow+CQAUEz2Xml39Qkv4PLulCikq6XCygEBcKKhA04O8/Hj2dEs9v9+qYUz
LyiQrpYiw4fFsbbNEbBf4xKULo3FjQCcDMUvzkRGK7griXMb8JADPAiAUIz3LjApKfzbNp4YEA1h
OYB/KjjJIdGnREnwZG60Rz6jncEHpWafbdyR6Jv4a73CyKot3J7Au5PZ9pBvb9iwr7pNzLkHAEzq
w26buK7U74YHAVCK8d7jMCoh/JDrRf21UEiIYHPf3OHfulbcamcJjhtGxUEj82R4b5WYYLQ7fQqb
d6f4ln1qrA5Wfi7ckaTirHvjhVYRp96FkQlKrra5CaDPX6+oQOkQ7z0zIwS3qzf0CgkWZWkEW/1G
u3/LWpmx04Pqn8zVYabX3m+0M3i7yORzm1ESgmk+hN8qS5fZ2KscB8YmKjnrv9hsx74qcblApkaG
OLnEW4ge0ueDK91svWdJUOTC62z/SAFWfxdW5ugEixOosvgPvKhv62HPszPUeHE4O3R8w9lmmOy+
D37enaqCRs5tcSputfPelvpFy6GTEXZehuKNS+JrBCMTWJ5ZGUXPec7uN6SU5nhT6YBo4Q5d9ouW
Y1qaMIahq0b/XjaTnYEUwK9GxeGdu5Ig83L+nGmw4YPLZr9tLMqK9ll/caudpZoqJb6NE3mxCk5V
9uQNGwqaOiAmBui4AnWR0/XcnQNke1NpdgjWP39YMzRGEA7Q0O7wvw1QijVDY7FykJ71yNrJ4Olv
GvzeSZSikuAeP7aPMw1sFTPJj306149JfFuZGWIim9sr2/2Zne5eEyCbFXUT5sELbwyJU2KGl3GE
M/EwBhW3+tGlGWCugdt1/cKJRlSYOv22/2ReDItruONYLdvB5I8DpKp9H5jZfcXiskKKhGydgr1T
UcImAEppurfEmKIW/qDjmuGxLPMsK9HA6WRdu882ktVSFHBE8r52oQV/LzX7rTdBJcHiAb7Z/7lG
G4wdbM0h0Y9/IlEl9dlek82JY37eJVykaKRcHKD7bGcP32KQ7L3KMrXC37wxJE6Jh/trA3OBAOmo
n0HL1snx3NF6fHVT17Y5KX5zphkbTjUHrHf1sFifwh8AHOJwMIG6ZBxfSIrinITutO+aeIdqM7Wc
2093iFiPjue6i64biSIec14zIg6fXrW4VKkQcaymHTYn5XTVjk5U4pvrbXj0QA0So6RoczCwdgZu
Ky9egWU5Or95Pr1q5pT4DX5OKSmlxKeaCABfXxdXHUxUSdHgGZnUPdfuQqDBnaJVEvEOQPbTybEy
LyYsDtDhoDhUzb1yJqX2+MMb2hywuoWC+0pSAK9N6uN37z/XYMPFJu64gQH6ALGSftoua7W7VFeR
oJKw1FBD1zM3AvDsVIrIX9pYPTzWJWOEoQ3sKOWWoMf1USFOEZz/Ye24BAyJ92/3eO+SkbOsUkKQ
G+gMYYD2z9SL99WYxCi3seja4m/CnQN4JLGPQGvkEvx6fAIvgc9X2nfVwrlyZBKCednRvOt5ZEA0
fjIkxm9/rxrt2HHZxFl+ZKLKL+cAjz4UimgPUErAErC74K4F8LJtC4kH+kdjtiF0gdDBULzpw6b+
0+GxLtUsQB2zDVr84a4+Afv6m1NNN4NG2HVMTPEfL2HtZAKqtUViGoS43v0mfG4BfNyuQuB3d/VB
nFKCULeBLRdbOLlAklqGl8Ym+C27ekQc3ro3xf/qBXCith27Sk0+DUczDf7D5Wssga+YvSpmjAAF
u82b8LkFRIoA4lVS/OWelJCNQiYbg9+dauKs+ydDY/HzMQkuH4RbmWEJSnw6JxMvjE0IOPk2B4PV
h+t89i87RoEhCf5d5hVG3xHHXaneKubBUupzbt3VQI8iDiZysez3ZGqwZnQ8Np5sDKn8lsIWzM2O
xsQ0duTyc6PisTBHhxO17XAwFEMSVRgUx9/J9T/HG1DW7Js9L8nVB6yjtMXOqTq6o0FEAnA4qc/2
3Q1BHqk2wkednx+TgLnZupDlgac+r0FTO3efU7Vy/HCADvNz9EFN/qdlJrx1rsVnmxoZweLBgQng
TG17gP67JsjYIc4polozx6GXm3AXAivcBUBbZ+QvPPjLtBTMztKGpBHUmDux7LNqwezqx2va8B9f
1Pptc2leDPRK/+pyaUsHmtodAfrvmhNjhzhc1+ZgvOe/ouuZuwxg8dyTIk8AMgnBW9PT8EBWdEhc
4ERNO1buvw5bmEexjte0YeHuSlj9xAvo5BI8NyYhYF35lVYEEgC9V6XQqGffgtb9JTJ3LaDOu0OV
ET7dCtwkghlpeCBLy3/g3NKnpSY8vLMSN0LcUzdfaMHcHRU3rYfwmX45MSng6geAfeVm/kQsAiq5
PZ91Xc/dOUC1d8YaS+QJALhJBDPTsXhwTEhEcOK6FdM+uoKDV/j72gvrbZj3zwr87MsaOAOEsd+R
psbyHwS+oLLG3ImjVfw5QDyPE0/BosbcyaW6VnePddcflNIyb4WorKkD41ODOxMoFGQSgv+blopU
rQy/O94QdPlacycW767EtH5a/GRkPMalqqHyCgo1djhx8IoZO0uM+Pwqv+8zJqlleGN6Gq+8Wwtb
bhITvz5rFPyPvfNFWXMHq30KWtb1d48ayNAy74tjS5vFDVfig+cnJGFQvArPHKh2WdSCxMErZhy8
YoaMEGTo5EjVyeFwUlSZOn1zOB8TppRJ8O7sdKTyCJWzORhsLmgG5SmU8qkzFJQ2d3BZdTkIgNIS
6kUBtwIBAMADA3XITcjCij1VKGzw4TQJMM4OUFxtseNqiAc0pRLgjZlpGJ/G75KMzQUtqLfwl0MS
1eLcRFra1MExNrSk6y93GaAYlDrc96TTNeIfXuCLAXFK7F/UH0+NiocUHCbZMLyKgZJGTvC3H/bF
gwMD6/wAYLQ58dqJ+qDa6Cdw+F0XTtewZBAHKC3uet5NAE3PD7WBotBdCGxuc6AyAufY+EIlk+BX
U1JwYHEWRqXwiC0UIOXGK7F/URam9ovm3c9Xjt1wrf4g2hkYhIGKLyqNdjS3sVTAwqbnh3WzUU+p
g6HHvVfWrcQFujA8WY0DS7Lwxqx09BPpgmopofjpuAR8sTQbgxL5H487XdOGd840Bt3ekCDaCKYv
HMR23D2P1+FQety7wNcVon69PCzMz4vFtz/OwQcP9cUdGZogVpzviVBKCZYMjcO3P87Bf09OYWkO
/mC0ObFi9zU4ncET3PAU4bWtrys4zj0y1IMAPCUPinxviSH/qrhx6+FCJiG4f4Ae9w/Qo9Jox85L
rfjyiglnrrfxjjlUyyWY2FeL+wfo8GBuDPQh6OMOhmLF7muoag1+y8zQK0TRAvKvWtgCIKX57v9l
+ULjN5wrBZDt/ts3KwZiUGJol0T0FmwOBkUNNpQ2daCipQNGm7Pb2ZKkkUOvlKJfrAIDEpSCvNt/
HajGu2dC82YuHBqH12dnCvr+RfXtmPR2iffPZU0vjRjg/gNL96CU7ifAM+6/7S0x3nYEoJJJMCJF
jREisFZvvHjwOt49HdrkA8B9WbqQy/rC3stGLgMQ63M/XJdE7fLeNz4pahV+1P4N4GAonv20Em+e
qPd71MxfUkqAqVn8NQy++ORSK4esgV3e+bjuCMoHRaO70HSxrh1F9eKdXrkd0dTmwIIPy/Hh2aaw
1Mx7+uugUQjrAyiqb8fFOlYMQqP3/g9wEEDzf490cHGBjwqaeDT93cCRCjOmvFmE/CvcUcLBpIXD
4gTv30fnmrja2tW8dhTLNMmp41CGbvXmHtsLmsP2s9/usNqd+MX+Kjz0QSlqjJ1hrXxQIEkjw3Se
1kW+sDkYbD/fzKVqbuXKz0kAzetH54OhFe57Vb25E3u/w7LAxxeaMe5PF/Hmt/Uh6flcafmowEGp
wWJvUSvqzSzirGhePzqfK7+f28Ip6xuBrx+90dvzEHEcuWrGfW8VYcX2K6g12gWZ+C6D0/IxiYL3
9/WjN7ja2+Qrv08XFKXYQkDXAei2URZct2L3xRbMyQvva523OhwMxYESI/58pA4nKsWxhP5obCL6
CHz6+shVMwqus85L2iiwxVcZv/wn7sVT7wNY7v27TiXF1AE6TOwXjYn9ojHwNrMR+MJ1ox0fnW3E
1tONqGoVzxWuU0lx7j+HQh8lrAv4gXeKcayCZbnd3LxhrM/vCfvtAaV0IzgIwNjuwMfnm/Hx+WYA
gF4lxcR+0RidocXoTA2Gp2qg5REvdyugsqUDn11qxScXm3HiWmT8Hs9OShF88o9cMeEodwjcRn/l
AkogsS+c2AmwLxkOhNykKAxKjsKINA2yE13/9hEp6iUY3DB34nSlBUevmvDFZSPKGgU8lcvD9ZAR
q8SJ1T+ASi5s+Nc9r1/EOTb739Xy23E/9FcuMBlSrEMIBFB8ox3FN9qxs6C5+zeNQoLsxCj0j1ei
f7wKGbFKZMYokBmnRKpOIeigNFkduNJkQ2VLBwpr21DaYMPZaitqTV7OGn7+IsHw8uxMwSf/H2cb
cY7zrgS6LlBZXjpI7H8d55QFhIZGIUWcRoZUnQIyKUHmzTP3GoUU8e4XVt6cNJuDcak8cK1sq51B
jdGOenMnOm5Bm8XMvFh8uHSgoHVaOpwY9/vzLg3FE5tbXhn/eKDyvDYiSrGeAAvhphEEBZ6rzGpz
wmpzourmUemjgg5V70IXJcUrDxoEr3fDgWrUsl3QNoCu51OeFy9qfWV8BWXoxlAdHmLG690u6Y/z
+iMtRtgvkZ+6ZsY7R+u4zL4bW343oYJPHUGIonQDdX14yCDoW/zbwDebWz6hD+YMFdbmb+lw4qlt
5XA4WVtdBYANfOsJyg4Z89zR6QD2B1Pmu44hqRp8/lPhpf7VO65g87d1XI9mtP5h4gG+9QTVq9Y/
TDwAis3iR+P2PssWIiVp5dj2o1zBJ/+fZxux+VgtV5ubg5l8IKgtwAUKuppQTMH3W4FfaBRSbH08
F2kxwoZ7X77Rjme3lfXsOD07TwUIVgdbX0iuKP2zRyYS0MMIgYC+C5BKCN5dmoM5wwMfHw8Gre0O
3PdqAUpvsIJzHCCY0vrHSUErTiHZaztOvFelHPeEhABTvJ9F2K4SOQSxhb2/PFfwyXc4KeZvuoRz
HM4pQvCr1tcm/TWUesNyRuv/4+t9AGaEU4eo6AVqfHlefzw1hd/p4WCw9N0ifHKOM/B0v/H1u2aG
Wm94LJxiPoBTAHLDqsezztsSUgnBe4/nYs4IYVc+APx8xxV8cpZz8otBMD+cusMOR9E/nZ8FiiMA
ksOt63aFRinFXx7LEWnyy7Hp0HWuR3UguNP458nl4dQvSDyS7sn8icRlH9CGXdlthiSdAltWDMKE
LGFj+wDg59vLselQNdcjC0BmGN+YHLa1XLCANN2qw7MIsAvfIc0gN1WDvz81BH3jhT3Y6XBSPPFu
ET45y3kzigPAbOOmKUHp+74gaESi7ieH5wHYhogRQe8JDA+N7oM/PTZQ8MCX1jYHFm0qxNHLrVyP
HQAWmt68+59CtSf4leC6lYciTASRhVImwW8fycYTd6UKXvflujYs+kshSm9wHsl3Tf5bwk0+IAIB
AIBuxaFZAN2GfzOZYEi6Fm88PghDM4R/rR2nbuCnH5TA6n5baA+Ds4Bgoentez4Tul3RPgqg+/FX
EwHswL+BdiCVEDx5bzrWP5QFmVTYIbPYnHhpexnez6/xlaUOBA+b3rlHlPAIUb8KEf2jr7II6B4I
aScQA35EieEGHf60LBdDM4Vf9afKjXjyvSKU1vm8haUYBLNN704NS9XzB3E/CwIg+okvtQTYjlAs
hiHIeEKJhXq1DOsfzsLSSamirPpf77yCt7+qdt3kzY39IJhvfm+qqKHKohNAF6If/2ItKF7CLS4c
SqUEK6em44U5/REjwtVt247VYd2OMtS0+Dx34ADB/5jfv5dXSFe4iBgBAED08i8mgmIrbkFXslRK
8MiEZPzsAQOy+gh/qcQ3xS14cVspznkc3GCt/goQssS8+d6IhUNGlAAAIHrZ5zGgeBURiDLmg+6J
f7CfOBNf1ILf7LqCI8UtgbJuBsFq85ZprZF8/4gTQBe0Sz+fTig2ISLcgL3PalQyLJ2cipX3Zgg+
8bZOBnvO1OO1vddwrsIUKHsFBVll+es0QSx7waLXCAAAtI8dVIHiRQKsQagh50FiQIoGK6dl4JGJ
yYhRC3tS6VK1BR9+XYO/H6tFfeALNm0ANlKCDZa/3ifeRwMDoFcJoAvaJQcNoFgL0OVi1B+vVWD2
6CQsnZKGsdnCOm0uVVmw50w9dp28gQuVvK/U2wxC1lu23lchxvsGg1uCALqgXXRgGBDaUTRvxGnl
mDkyEbNGJWHasHio5MLY7K81tONUqRGHLjbhUGEzqhoD3J3kufvsAsE6y9+mF4gzgsHjliKALmgf
PZAH0DUI8TRSkl6JhyckY1C6FgNTNUiLV6FvkEfYrzW043qTDZdrrCitsaKkxopTZUY0m4O+CNIG
gm0ANlo+mnGxt8bUF25JAuiC9tH9yaBYBmAV/AmLPK0/cdFyaFUyJOkVUHndzOVwUtQ022DrZFAv
zN0AFSDYBGCLZduMurBrEwm3NAG4Q/vIvskAloBiLgDhQ2+EQSNcbH6r5e8z88OuLQK4bQigC5pH
9slAMRnAXEIxA17X2vYCyijBfriCYfKt/5gZ2Q8uhonbjgC8oZm/1wBgMijGAxgPYAjEMzc7ABQC
OA6C4wDyrdvvr+jtMQgHtz0BeEPz8F4VXN7HHADZoMgGkA6XW1oLUEOAKirgirmrA1ANgjK4vrFT
AqDYuuP+XtPZv8f3+B7fQ1j8P44rfopLvTtSAAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDE4LTA4LTIx
VDAxOjQzOjMwLTA3OjAw87aoXwAAACV0RVh0ZGF0ZTptb2RpZnkAMjAxOC0wOC0yMVQwMTo0NDow
OC0wNzowMN1XQh4AAAAASUVORK5CYII=" /></svg>论坛</div></a></a><a href="https://github.com/loliMay/deepin-develop-guide" target="_blank"><div class="icon-button"><svg aria-labelledby="simpleicons-github-dark-icon" lang="" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title id="simpleicons-github-icon" lang="en">GitHub Dark icon</title><path fill="#333" d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"></path></svg>GITHUB</div></a>
<h1 class="title">Contributors

[<img alt="nujhong" src="https://avatars3.githubusercontent.com/u/32427260?s=460&v=4&s=117" width="117">](https://github.com/lolimay)[<img alt="zhangzhengyi12" src="https://avatars3.githubusercontent.com/u/18530271?s=460&v=4&s=117" width="117">](https://github.com/ziqiangxu)</h1>
<p><a href="https://github.com/loliMay/deepin-develop-guide#user-content-%E5%8F%82%E4%B8%8E%E5%86%99%E4%BD%9C%E6%A0%A1%E5%AF%B9">Join us and become contributor</a></p>
</div>

<style>
    .title {
        margin:0;
        padding: 50px 0 0 0;
        text-align: center;
        font-size: 32px;
        font-family: "Source Sans Pro", "Helvetica Neue", Arial, sans-serif;
        color: #34495e;
    }
    .intro {
        color: #666;
        font-size: 18px;
        padding: 0 100px;
        text-indent: 2em;
        margin:0;
    }
    .indent {
        text-indent:4em;
    }
    .button-box {
        margin:40px 0 80px 0;
        text-align: center;
    }
    .homepage-button, .icon-button {
        display: inline-block;
        border-radius: 30px;
        font-weight: 600;
    }
    .homepage-button {
        margin:0;
        color: #4fc08d;
        background: #fff;
        border: 1px solid  #4fc08d;
        padding: 5px 30px;
        margin-right: 20px;
    }
    .homepage-button:hover {
        color: #fff;
        background: #4fc08d;
    }
    .icon-button {
        padding: 5px 20px;
        background: rgba(246, 246, 246, 1);
        color: #7f8c8d;
        position: relative;
        padding-left: 3em;
        transition: .5s all;
        margin-right: 20px;
        font-weight: 500;
    }
    .icon-button>svg {
        width: 1.5em;
        position: absolute;
        top: 0.4em;
        left: 0.8em;
    }
    .icon-button:hover {
        color: #7e8a8a;
        background: rgba(241, 241, 241, 1.0);
        box-shadow: 0 0 5px 0 #ccc;
        color:#777;
    }
@media (max-width: 1700px) {
    .intro {
        padding: 0 40px;
    }
}
@media (max-width: 450px) {
    .intro {
        padding: 0;
        text-indent:0;
    }
    .indent {
        text-indent:2em;
    }
    .title {
        padding:10px 0;
        font-size:30px;
        line-height:1.8;
    }
    .button-box {
        margin: 80px 0;
    }
    #forum-button {
        display:none;
    }
}
@media (max-height:800px) {
    .button-box {
        margin-bottom:300px;
    }
}
@media (max-height:700px) {
    .button-box {
        margin-bottom:200px;
    }
}
</style>