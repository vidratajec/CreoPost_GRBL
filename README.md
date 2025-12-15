# CreoPost GRBL
Creo CAM postprocessor compatible with GRBL

move:


-uncx01.s02

-uncx01.f02

-uncx01.p02

-uncx01.p02.txt


to
...\PTC\Creo 9.0.6.0\Common Files\x86e_win64\gpost


start and end sections of gcode are hardcodes as:

--start-
G21

G90

M3 S1000

--------


--end--

G1 Z1.0

M5

-------

Other:
    All codes should be (are) non modal.
    G2/G3 should use +/-R for angles <180deg and IJ for 360deg
    M/T codes are not supported

