Tema2

Lidia Istrate 342C4


Task 1:
- dillation: dupa claculul noii imagini prin sobel + binarizare, 
locatiile in care pixelii au devenit albi, vor fi colorati cu negru in imaginea originala
functii folosite : get_dillation_image, get_binarisation_image, get_sobel_image

Task 2:
apply_colors_intervals
get_value_from_intervals : am definit 8 intervale si pentru fiecare interval returnez valoarea de mijloc

Task 3:
apply_extend_segmentation : folosesc pixel_region pentru a stoca numarul regiunii alese pt pixeli, regions pentru a stoca regiunile sub forma [sum_red, sum_green, sum_blue, numar_pixeli_in_regiune]
apply_formula_region_gray : pt imagini gray
apply_formula_region : pentru imagini rgb,
	am folosit formula | R - Rp | + | G - Gp | + | B - Bp | <= threshold
		unde (Rp, Gp, Bp) valorile pixelului si  (R, G, B) media aritmetica a regiunii

Initial pot fi alese optiunile de micsorare a paletei de culori prin I (task2), S(task3) sau deloc, apoi se aplica dilatarea si apoi se pate alege din nou paleta de culori