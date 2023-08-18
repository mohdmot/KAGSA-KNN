<h1 align="center">KAGSA KNN</h1>
<p align="center">
<img src="https://github.com/Zaky202/KAGSA-KNN/blob/main/image.png?raw=true" height="300">
</p>

<p align="center">a simple KNN algorithm in KAGSA Programming Language</p>

## Test
i use this small dataset that have `[Cigarettes, Weight]` in `X` and `[0:Bad , 1:Good]` in `y`.
| i. | Cigarettes | Weight |   |
| -  |:----------:|:------:|:-:|
| 0  |      7     |   70   | 0 |
| 1  |      7     |   40   | 0 |
| 2  |      3     |   40   | 1 |
| 3  |      1     |   40   | 1 |
| 4  |      3     |   70   | 0 |

`cigarettes.kg` :
```js
include "KNeighbors.kgl"

// X : [Cigarettes, Weight]
// y : [0:Bad , 1:Good]
data = ``{
    "x": [[7,70],[7,40],[3,40],[1,40],[3,70]],
    "y": [0,0,1,1,0],
    "k":2
}``
data = JSON.parse(data)
new_x = list(7,50)

pred = KNeighbors.KNN(data.k ,data.x , data.y, new_x)
if pred {
    write 'Good'
}else {
    write 'Bad'
}
```
