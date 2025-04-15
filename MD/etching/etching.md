# Травление

```mermaid
flowchart
	n9["Травление"]

	n9 --- n18@{ shape: "stadium", label: "Защита меди" }
	n18 --- n12["Фоторезист"]
		click n12 "https://github.com/ufrs12/PCB-making/blob/main/MD/etching/photorez/photorez.md"

	n18 --- n13["ЛУТ"]
	n18 --- n14["Маркер/лак"]
	n18 --- n17["Красим/жгем"]

	n9 --- n19@{ shape: "stadium", label: "Травление" }
	n19 --- n20["Хлорное железо"]
	n19 --- n21["Перекись и лимонная кислота"]

	n9 --- n22@{ shape: "stadium", label: "Удаление защитного слоя" }
