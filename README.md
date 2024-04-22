# MFFNet
https://yzueducn-my.sharepoint.com/:f:/g/personal/zhangxf_yzu_edu_cn/En3cINAQgXJFjvUIw8Qg7zUBWcmI9NwXW7VwsToAuLoLrg?e=nm6ete.

![img1](./img/1.svg)

<div style="text-align:center;">
    <p>fig1</p>
</div>


![img2](./img/2.svg)

<div style="text-align:center;">
    <p>fig2</p>
</div>

![img3](./img/3.svg)

<div style="text-align:center;">
    <p>fig3</p>
</div>

![img4](./img/4.svg)

<div style="text-align:center;">
    <p>fig4</p>
</div>


|      |                       |                                 |           Components            |                    |                    |         |      |           |           |    SHT B    |    ->    |      SHT A      |              |
| :--: | :-------------------: | :-----------------------------: | :-----------------------------: | :----------------: | :----------------: | :-----: | :--: | :-------: | :-------: | :---------: | :------: | :-------------: | :----------: |
|  SN  | $FB_{\frac{1}{4}->1}$ | $FB_{\frac{1}{4}->\frac{1}{2}}$ | $FB_{\frac{1}{4}->\frac{1}{4}}$ | $FM_{\frac{1}{2}}$ | $FM_{\frac{1}{4}}$ | MCA/CNN | Loss |    MAE    |    MSE    | Params (MB) | TCE (ep) | Train Time(min) | Test Time(s) |
|  1   |           √           |                ×                |                ×                |         ×          |         ×          |   MCA   | +BS  |   158.7   |   258.7   |    67.49    |   100    |      48.2       |      34      |
|  2   |           √           |                √                |                ×                |         ×          |         ×          |   MCA   | +BS  |   139.4   |   247.5   |    68.82    |   130    |      57.6       |      26      |
|  3   |           √           |                √                |                √                |         ×          |         ×          |   MCA   | +BS  |   139.9   |   235.0   |    68.86    |   320    |      137.6      |      27      |
|  4   |           √           |                √                |                √                |         √          |         ×          |   MCA   | +BS  |   127.9   |   209.4   |    68.86    |   110    |      49.5       |      26      |
|  5   |           √           |                √                |                √                |         √          |         √          |   CNN   | +BS  |   133.3   |   255.8   |    68.76    |   320    |      112.0      |      19      |
|  6   |           √           |                √                |                √                |         √          |         √          |   MCA   | MSE  |   130.3   |   216.0   |    68.86    |   800    |      640.0      |      45      |
|  7   |           √           |                √                |                √                |         √          |         √          |   MCA   | +BS  | **107.3** | **188.5** |    68.86    |   100    |      84.0       |      32      |
|  8   |                       |                                 |              FIDTM              |                    |                    |         |      |   147.6   |   282.2   |    66.58    |   670    |      335.0      |      21      |



<table>
<thead>
  <tr>
    <th rowspan="2">SN</th>
    <th colspan="7">Component</th>
    <th colspan="6">SHT B -&gt; SHT A</th>
  </tr>
  <tr>
    <th>$FB_{\frac{1}{4}-&gt;1}$</th>
    <th>$FB_{\frac{1}{4}-&gt;1}$</th>
    <th>$FB_{\frac{1}{4}-&gt;\frac{1}{4}}$</th>
    <th>$FM_{\frac{1}{2}}$</th>
    <th>$FM_{\frac{1}{4}}$</th>
    <th>MCA/CNN</th>
    <th>Loss</th>
    <th>MAE</th>
    <th>MSE</th>
    <th>Params<br>(MB)</th>
    <th>TCE<br>(ep)</th>
    <th>Train Time<br>(min)</th>
    <th>Test Time<br>(s)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>1</td>
    <td>√</td>
    <td>×</td>
    <td>×</td>
    <td>×</td>
    <td>×</td>
    <td>MCA</td>
    <td>+BS</td>
    <td>158.7</td>
    <td>258.7</td>
    <td>67.49</td>
    <td>100</td>
    <td>48.2</td>
    <td>34</td>
  </tr>
  <tr>
    <td>2</td>
    <td>√</td>
    <td>√</td>
    <td>×</td>
    <td>×</td>
    <td>×</td>
    <td>MCA</td>
    <td>+BS</td>
    <td>139.4</td>
    <td>247.5</td>
    <td>68.82</td>
    <td>130</td>
    <td>57.6</td>
    <td>26</td>
  </tr>
  <tr>
    <td>3</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>×</td>
    <td>×</td>
    <td>MCA</td>
    <td>+BS</td>
    <td>139.9</td>
    <td>235.0</td>
    <td>68.86</td>
    <td>320</td>
    <td>137.6</td>
    <td>27</td>
  </tr>
  <tr>
    <td>4</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td></td>
    <td>MCA</td>
    <td>+BS</td>
    <td>127.9</td>
    <td>209.4</td>
    <td>68.86</td>
    <td>110</td>
    <td>495</td>
    <td>26</td>
  </tr>
  <tr>
    <td>5</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>CNN</td>
    <td>+BS</td>
    <td>133.3</td>
    <td>255.8</td>
    <td>68.76</td>
    <td>320</td>
    <td>112.0</td>
    <td>19</td>
  </tr>
  <tr>
    <td>6</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>MCA</td>
    <td>MSE</td>
    <td>130.3</td>
    <td>216.0</td>
    <td>68.86</td>
    <td>800</td>
    <td>640.0</td>
    <td>45</td>
  </tr>
  <tr>
    <td>7</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>MCA</td>
    <td>+BS</td>
    <td>107.3</td>
    <td>188.5</td>
    <td>68.86</td>
    <td>100</td>
    <td>84.0</td>
    <td>32</td>
  </tr>
  <tr>
    <td>8</td>
    <td colspan="7">FIDTM</td>
    <td>147.6</td>
    <td>282.2</td>
    <td>66.58</td>
    <td>670</td>
    <td>335.0</td>
    <td>21</td>
  </tr>
</tbody>
</table>
