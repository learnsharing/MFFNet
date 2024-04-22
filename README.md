# MFFNet
https://yzueducn-my.sharepoint.com/:f:/g/personal/zhangxf_yzu_edu_cn/En3cINAQgXJFjvUIw8Qg7zUBWcmI9NwXW7VwsToAuLoLrg?e=nm6ete.

![img1](./img/1.svg)
<center>
fig1
</center>

![img2](./img/2.svg)
<center>
fig2
</center>

![img3](./img/3.svg)
<center>
fig3
</center>

![img4](./img/4.svg)
<center>
fig4
</center>

|  SN  |                          Components                          |                        SHT B -> SHT A                        |
| :--: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|      | $FB_{\frac{1}{4}->1}$     $FB_{\frac{1}{4}->\frac{1}{2}}$    $FB_{\frac{1}{4}->\frac{1}{4}}$    $FM_{\frac{1}{2}}$    $FM_{\frac{1}{4}}$    MCA/CNN     Loss | MAE         MSE    Params(MB)    TCE(ep)   Train Time(min)   Test Time(s) |
|  1   | √                ×               ×           ×            ×           ×             MCA           +BS | 158.7       258.7      67.49              100                 48.2                      34 |
|  2   | √                √               ×           ×            ×           ×             MCA           +BS | 139.4       247.5      68.82              130                 57.6                      26 |
|  3   | √                √               √           √            ×           ×             MCA           +BS | 139.9       235.0      68.86              320                 137.6                    27 |
|  4   | √                √               √           √            √           ×             MCA           +BS | 127.9       209.4      68.86              110                 49.5                      26 |
|  5   | √                √               √           √            √           √             CNN           +BS | 133.3       255.8      68.76              320                 112.0                    19 |
|  6   | √                √               √           √            √           √             MCA           MSE | 130.3       216.0      68.86              800                 640.0                    45 |
|  7   | √                √               √           √            √           √             MCA           +BS | 107.3       188.5      68.86              100                 84.0                      32 |
|  8   |                            FIDTM                             | 147.6       282.2      66.58              670                 335.0                    21 |
