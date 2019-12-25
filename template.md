## F, Balanced Path
### Difficulty

### Statement
$H$ x $W$のグリッド上を$(1,1)$から$(H, W)$まで最短経路で辿りながら、

$A_{ij}$を足すか引くか選んでいく。累積の絶対値の最小値は何か。

### Constraints
- $ 2 \leq H, W \leq 80 $
- $ -80 \leq A_i \leq 80 $

### Editorial
各マス$i$が値$j$を取りうるかを管理するDPで解く。

$O(n^4)$をやることになり時間制約が厳しいので、bitset高速化を行う。
