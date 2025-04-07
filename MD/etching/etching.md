# Травление

```mermaid
flowchart
	n9["Травление"]
	n9 --- n18@{ shape: "circle", label: "Защита меди" }
	n18 --- n12["Фоторезист"]
	n18 --- n13["ЛУТ"]
	n18 --- n14["Маркер/лак"]
	n18 --- n17["Красим/жгем"]

	n12 --- n15["Пленочный"]
	n12 --- n16["Жидкий"]

	n19@{ shape: "circle", label: "Травление" }
	n9 --- n19
	n19 --- n20["Хлорное железо"]
	n19 --- n21["Перекись и лимонная кислота"]
	n22@{ shape: "circle", label: "Удаление защитного слоя" }
	n18
	n22
	n9 --- n22@{ shape: "circle", label: "Удалениезащитного слоя" }
	n22@{ shape: "circle", label: "Удаление защиты" }
	
	n22 --- n24["Зависит от варианта защиты меди"]
	n27@{ shape: "circle", label: "Приобретение" }
	n15 --- n27
	n28@{ shape: "circle", label: "Хранение" }
	n15 --- n28
	n29@{ shape: "circle", label: "Раскрой" }
	n15 --- n29
	n31@{ shape: "circle", label: "Подготовка заготовки" }
	n15 --- n31
	n16 --- n32
	n32@{ shape: "circle", label: "Приобретение" }
	n16 --- n38@{ shape: "circle", label: "Хранение" }
	n39@{ shape: "circle", label: "Подготовка заготовки" }
	n16 --- n39
	n15 --- n40@{ shape: "circle", label: "Нанесение" }
	n41@{ shape: "circle", label: "Нанесение" }
	n16 --- n41
	n15 --- n30@{ shape: "circle", label: "Экспонирование" }
		click n30 "https://github.com/ufrs12/PCB-making/blob/main/MD/expo/expo.md"
	n15 --- n33@{ shape: "circle", label: "Проявка" }
	n16 --- n34@{ shape: "circle", label: "Экспонирование" }
		click n34 "https://github.com/ufrs12/PCB-making/blob/main/MD/expo/expo.md"
	n16 --- n35@{ shape: "circle", label: "Проявка" }
