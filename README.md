# Binary-Space-Partition-Dungeon-Generator

在Unity2022中，利用二叉树空间分割实现生成2D随机地牢。

### 最终效果

![](https://github.com/guobarou/Binary-Space-Partition-Dungeon-Generator/blob/main/Assets/Art/Images/end.png)

## 第1步 空间分割

该算法的想法是从代表整个地牢的矩形单元格开始。然后我们将这个地下城分成两个子地牢，随机选择分割位置，该过程将以递归方式对每个子地下城重复，直到子地下城大约达到房间的所需大小。

![](https://github.com/guobarou/Binary-Space-Partition-Dungeon-Generator/blob/main/Assets/Art/Images/1.png)

## 第2步 生成房间编号

根据二叉节点索引生成所有房间编号，生成得房间为不可再分割得最终节点。

![](https://github.com/guobarou/Binary-Space-Partition-Dungeon-Generator/blob/main/Assets/Art/Images/2.png)

## 第3步 生成所有节点

房间只需要显示最终不可分割得节点，但是我们可以通过最大节点得到一个完整得二叉树。

![](https://github.com/guobarou/Binary-Space-Partition-Dungeon-Generator/blob/main/Assets/Art/Images/3.png)

## 第4步 生成房间编号

通过完整得二叉树，逐级向上合并，等到更加合理得走廊。

![](https://github.com/guobarou/Binary-Space-Partition-Dungeon-Generator/blob/main/Assets/Art/Images/4.png)

## 第5步 围墙

利用二进制存储围墙周围8方向信息，二进制运算得到合理得围墙角度。

![](https://github.com/guobarou/Binary-Space-Partition-Dungeon-Generator/blob/main/Assets/Art/Images/5.png)

# All used with permission/license
https://pixel-poem.itch.io/dungeon-assetpuck

