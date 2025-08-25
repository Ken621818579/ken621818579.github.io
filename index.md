# Hello world!

广州地铁(羊角）你还有多少版本的地铁图是我不知道的😅
翻遍了我能想到的简中搜索引擎和Github，找到这些版本：
https://appmsg.gzmtr.cn/DNSFile/Modules/gzmtrmapv241.jpg
https://cs.gzmtr.com/ckfw/road.jpg
https://cs.gzmtr.com/ckfw/xlu_2020/202011/W020201209350245548608.jpg
https://cs.gzmtr.com/ckfw/xlu_2020/202011/W020220421601916560440.jpg
https://cs.gzmtr.com/ckfw/xlu_2020/202011/W020221227789185419694.png
https://cs.gzmtr.com/ckfw/xlu_2020/202011/W020221227789185419694.png
https://cs.gzmtr.com/ckfw/xlu_2020/202011/W020230130620477475552.png
https://cs.gzmtr.com/ckfw/xlu_2020/202011/W020231227816642640987.png
https://cs.gzmtr.com/ckfw/xlu_2020/202401/W020240120824181860073.png
https://cs.gzmtr.com/ckfw/xlu_2020/202405/W020240524846059965254.png
https://cs.gzmtr.com/ckfw/xlu_2020/202405/W020240527599125758205.png
https://cs.gzmtr.com/ckfw/xlu_2020/202406/W020240607636823912423.png
https://cs.gzmtr.com/ckfw/xlu_2020/202409/W020241002000760177182.png
https://cs.gzmtr.com/ckfw/xlu_2020/202411/W020241115612240871255.png
https://cs.gzmtr.com/ckfw/xlu_2020/202412/W020241228010203039845.png
https://cs.gzmtr.com/ckfw/xlu_2020/202412/W020241228010311222828.png
https://cs.gzmtr.com/ckfw/xlu_2020/202412/W020241228010364924615.png
https://cs.gzmtr.com/ckfw/xlu_2020/202506/W020250620526298753932.png
https://cs.gzmtr.com/ckfw/xlu_2020/202506/W020250630720140685324.png
https://cs.gzmtr.com/ckfw/xlu_2020/202506/W020250813808772963251.png
https://cs.gzmtr.com/ckfwEnglish/xlu_2020/202410/W020241031720239138030.png
https://cs.gzmtr.com/ckfwEnglish/xlu_2020/202506/W020250814397545829913.png
如果你有任何其他版本（最好是官网的URL，或者是文件名形如“W0+8位日期+12位随机数字”的历史版本），欢迎Issue/Pull Request/email 621818579@qq.com !

要计算金属丝的杨氏模量（Young's modulus），我们可以利用胡克定律和杨氏模量的定义公式。以下是详细的计算步骤：

### 1. 杨氏模量的定义
杨氏模量 \( E \) 的定义为：
\[
E = \frac{\text{应力}}{\text{应变}} = \frac{F/A}{\Delta L / L_0}
\]
其中：
- \( F \) 是施加的力（单位：N），
- \( A \) 是金属丝的横截面积（单位：m²），
- \( \Delta L \) 是金属丝的伸长量（单位：m），
- \( L_0 \) 是金属丝的原始长度（单位：m）。

### 2. 计算横截面积 \( A \)
金属丝的直径 \( d = 0.19 \, \text{mm} = 0.00019 \, \text{m} \)，因此半径 \( r = \frac{d}{2} = 9.5 \times 10^{-5} \, \text{m} \)。

横截面积：
\[
A = \pi r^2 = \pi (9.5 \times 10^{-5})^2 \approx 2.835 \times 10^{-8} \, \text{m}^2
\]

### 3. 数据处理
将砝码质量 \( m \)（单位：kg）转换为力 \( F = m \cdot g \)，其中 \( g = 9.80 \, \text{m/s}^2 \)。伸长量 \( \Delta L \) 为原始读数减去初始读数（这里假设初始读数为挂 100 g 砝码时的读数 2.95 mm，但通常初始读数应为未加载时的读数。如果题目未给出初始长度，可能需要调整计算方法）。

不过，从数据来看，随着砝码质量的增加，读数在减小（可能是反向测量系统），因此伸长量 \( \Delta L \) 可能是 \( L_0 - L \)，其中 \( L \) 是当前读数。假设原始长度 \( L_0 = 2.95 \, \text{mm} \)，则 \( \Delta L = L_0 - L \)。

但更合理的方法是拟合 \( F \) 与 \( \Delta L \) 的关系，计算斜率 \( k = \frac{F}{\Delta L} \)，然后代入杨氏模量公式：
\[
E = \frac{F \cdot L_0}{A \cdot \Delta L} = \frac{k \cdot L_0}{A}
\]

### 4. 计算 \( F \) 和 \( \Delta L \)
将数据整理如下（假设 \( L_0 = 2.95 \, \text{mm} \) 为初始长度）：

| 砝码质量 \( m \) (g) | 力 \( F = m \cdot g \) (N) | 读数 \( L \) (mm) | 伸长量 \( \Delta L = L_0 - L \) (mm) |
|----------------------|---------------------------|-------------------|--------------------------------------|
| 100                  | 0.980                     | 2.95              | 0                                    |
| 300                  | 2.94                      | 2.725             | 0.225                                |
| 500                  | 4.90                      | 2.525             | 0.425                                |
| 700                  | 6.86                      | 2.275             | 0.675                                |
| 900                  | 8.82                      | 2.025             | 0.925                                |
| 1100                 | 10.78                     | 1.80              | 1.15                                 |
| 1300                 | 12.74                     | 1.60              | 1.35                                 |
| 1500                 | 14.70                     | 1.375             | 1.575                                |

### 5. 拟合 \( F \) 与 \( \Delta L \) 的关系
绘制 \( F \)（y 轴）与 \( \Delta L \)（x 轴）的曲线，计算斜率 \( k \)：
\[
k = \frac{\Delta F}{\Delta (\Delta L)}
\]

选择两点计算斜率：
- 第一点：\( F = 2.94 \, \text{N} \), \( \Delta L = 0.225 \, \text{mm} = 2.25 \times 10^{-4} \, \text{m} \)
- 最后一点：\( F = 14.70 \, \text{N} \), \( \Delta L = 1.575 \, \text{mm} = 1.575 \times 10^{-3} \, \text{m} \)

斜率：
\[
k = \frac{14.70 - 2.94}{1.575 \times 10^{-3} - 2.25 \times 10^{-4}} = \frac{11.76}{1.35 \times 10^{-3}} \approx 8711.1 \, \text{N/m}
\]

### 6. 计算杨氏模量 \( E \)
原始长度 \( L_0 = 76 \, \text{cm} = 0.76 \, \text{m} \)，横截面积 \( A \approx 2.835 \times 10^{-8} \, \text{m}^2 \)。

杨氏模量：
\[
E = \frac{k \cdot L_0}{A} = \frac{8711.1 \times 0.76}{2.835 \times 10^{-8}} \approx 2.335 \times 10^{11} \, \text{Pa}
\]

### 7. 结果
杨氏模量约为：
\[
E \approx 2.34 \times 10^{11} \, \text{Pa} \, (\text{或} \, 234 \, \text{GPa})
\]

### 注意事项
1. 如果初始长度 \( L_0 \) 不是 2.95 mm，而是金属丝的原长（76 cm），则需要重新计算 \( \Delta L \)。
2. 如果读数表示的是金属丝的绝对伸长量（而非反向测量），则 \( \Delta L \) 的计算方式会不同。
3. 更精确的方法是使用最小二乘法拟合所有数据点求斜率 \( k \)。

如果问题描述中读数表示的是金属丝的伸长量（即 \( \Delta L = \text{读数} \)），则需重新计算。请确认读数的具体含义。
