# PCB-making
## Дорожная карта изготовления печатных плат

В диаграмме овалами или кругами обозначены процедуры, необходимые для выполнения на этом этапе, их следует выполнять, как правило, слева направо. Прямоугольниками отображаются варианты, из которых требуется выбрать один.

```mermaid
flowchart
	n10@{ shape: "stadium", label: "Работа с проектом" }
		click n10 "https://github.com/ufrs12/PCB-making/blob/main/MD/project/project.md"
	n10 --- n2["Жесткая"]
	n10 --- n3["Гибкая"]

	n2 --- n7["Фольгированный
стеклотекстолит"]
	n2 --- n8["Другие варианты,
включая изготовление
собственных материалов"]
	
	n7 --- n4["Односторонняя"]
	n7 --- n5["Двухсторонняя"]
	n7 --- n6["Многослойная"]
	
	n4 --- n25@{ shape: "stadium", label: "Приобретение
стеклотекстолита" }
	n4 --- n26@{ shape: "stadium", label: "Хранение
стеклотекстолита" }
	n4 --- n23@{ shape: "stadium", label: "Раскрой
стеклотекстолита" }
	n4 --- n9@{ shape: "stadium", label: "Формирование
медного слоя" }
		click n9 "https://github.com/ufrs12/PCB-making/blob/main/MD/cu_layer/Cu_layer.md"

	n9 --- n13["Паяльная маска"]
	n9 --- n14["Без паяльной маски"]
	
	n13 --- n15@{ shape: "f-circ" }
	n14 --- n15
	n15 --- n17["Лужение"]
	n15 --- n18["Без лужения"]
	n17 --- n16["Сверловка"]
	n18 --- n16
	n16 --- n1["Трафарет для
паяльной пасты"]
		click n1 "https://github.com/ufrs12/PCB-making/blob/main/MD/%20stencil/stencil.md"
	n16 --- n11["Без трафарета"]
