# Anywhy Flake Keyboard Wiring Diagram

## Matrix Layout and Pin Connections

The Anywhy Flake keyboard uses a matrix layout with rows and columns. Each key is at the intersection of a row and column. The diode direction is `col2row`, meaning diodes should be placed with the cathode (marked end/black bar) facing the column pins.

### Left Half Matrix (nice!nano v2)

```
                    COL0    COL1    COL2    COL3    COL4    COL5
                    PIN2    PIN3    PIN4    PIN5    PIN6    PIN7
                    
ROW0 (PIN8)         ESC     UNLOCK  2       3       4       5
ROW1 (PIN9)         ENTER   Q       W       E       R       T
ROW2 (PIN10)        TAB     A       S       D       F       G
ROW3 (PIN16)        [       Z       X       C       V       B
ROW4 (PIN14)        -       LGUI    LALT    LCTRL   SPACE   MO(1)
```

### Right Half Matrix (nice!nano v2)

```
                    COL0    COL1    COL2    COL3    COL4    COL5
                    PIN14   PIN15   PIN18   PIN19   PIN20   PIN21
                    
ROW0 (PIN16)        6       7       8       9       0       -
ROW1 (PIN10)        Y       U       I       O       P       BSPC
ROW2 (PIN9)         H       J       K       L       ;       '
ROW3 (PIN8)         N       M       ,       .       /       ]
ROW4 (PIN7)         MO(2)   LSHFT   LGUI    LALT    LCTRL   -
```

## Visual Keyboard Layout with Pin Connections

```
┌─────────┬─────────┬─────────┬─────────┬─────────┬─────────┐      ┌─────────┬─────────┬─────────┬─────────┬─────────┬─────────┐
│ ESC     │ UNLOCK  │ 2       │ 3       │ 4       │ 5       │      │ 6       │ 7       │ 8       │ 9       │ 0       │ -       │
│ R0C0    │ R0C1    │ R0C2    │ R0C3    │ R0C4    │ R0C5    │      │ R0C0    │ R0C1    │ R0C2    │ R0C3    │ R0C4    │ R0C5    │
│ P8-P2   │ P8-P3   │ P8-P4   │ P8-P5   │ P8-P6   │ P8-P7   │      │ P16-P14 │ P16-P15 │ P16-P18 │ P16-P19 │ P16-P20 │ P16-P21 │
├─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤      ├─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ ENTER   │ Q       │ W       │ E       │ R       │ T       │      │ Y       │ U       │ I       │ O       │ P       │ BSPC    │
│ R1C0    │ R1C1    │ R1C2    │ R1C3    │ R1C4    │ R1C5    │      │ R1C0    │ R1C1    │ R1C2    │ R1C3    │ R1C4    │ R1C5    │
│ P9-P2   │ P9-P3   │ P9-P4   │ P9-P5   │ P9-P6   │ P9-P7   │      │ P10-P14 │ P10-P15 │ P10-P18 │ P10-P19 │ P10-P20 │ P10-P21 │
├─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤      ├─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ TAB     │ A       │ S       │ D       │ F       │ G       │      │ H       │ J       │ K       │ L       │ ;       │ '       │
│ R2C0    │ R2C1    │ R2C2    │ R2C3    │ R2C4    │ R2C5    │      │ R2C0    │ R2C1    │ R2C2    │ R2C3    │ R2C4    │ R2C5    │
│ P10-P2  │ P10-P3  │ P10-P4  │ P10-P5  │ P10-P6  │ P10-P7  │      │ P9-P14  │ P9-P15  │ P9-P18  │ P9-P19  │ P9-P20  │ P9-P21  │
├─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤      ├─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ [       │ Z       │ X       │ C       │ V       │ B       │      │ N       │ M       │ ,       │ .       │ /       │ ]       │
│ R3C0    │ R3C1    │ R3C2    │ R3C3    │ R3C4    │ R3C5    │      │ R3C0    │ R3C1    │ R3C2    │ R3C3    │ R3C4    │ R3C5    │
│ P16-P2  │ P16-P3  │ P16-P4  │ P16-P5  │ P16-P6  │ P16-P7  │      │ P8-P14  │ P8-P15  │ P8-P18  │ P8-P19  │ P8-P20  │ P8-P21  │
└─────────┴─────────┼─────────┼─────────┼─────────┼─────────┤      ├─────────┼─────────┼─────────┼─────────┼─────────┴─────────┘
                    │ LGUI    │ LALT    │ LCTRL   │ SPACE   │      │ MO(2)   │ LSHFT   │ LGUI    │ LALT    │ LCTRL   │
                    │ R4C1    │ R4C2    │ R4C3    │ R4C4    │      │ R4C0    │ R4C1    │ R4C2    │ R4C3    │ R4C4    │
                    │ P14-P3  │ P14-P4  │ P14-P5  │ P14-P6  │      │ P7-P14  │ P7-P15  │ P7-P18  │ P7-P19  │ P7-P20  │
                    └─────────┴─────────┴─────────┼─────────┤      ├─────────┼─────────┴─────────┴─────────┘
                                                  │ MO(1)   │      │ MO(2)   │
                                                  │ R4C5    │      │ R4C0    │
                                                  │ P14-P7  │      │ P7-P14  │
                                                  └─────────┘      └─────────┘
```

## Wiring Instructions

1. **For each key**:
   - Connect one terminal of the switch to the corresponding row pin
   - Connect the other terminal to the cathode (marked end) of a diode
   - Connect the anode of the diode to the corresponding column pin

2. **Diode Direction**:
   - The black bar/cathode of the diode should face toward the column pin
   - The unmarked end/anode of the diode connects to the key switch

3. **Pin Notation**:
   - Format is `RowPin-ColumnPin` (e.g., `P8-P2` means row pin 8, column pin 2)
   - These are GPIO numbers on the nice!nano, not physical pin numbers

## nice!nano v2 Pin Mapping

When wiring your keyboard, you'll need to connect to the physical pins on the nice!nano that correspond to these GPIO numbers. Refer to the nice!nano pinout diagram to locate the correct physical pins.

## Notes

- The internal pull-down resistors are enabled for the rows, so you don't need external pull-down resistors
- The keyboard uses a split design with separate controllers for left and right halves
- Make sure to follow the diode direction correctly (col2row means cathode toward column)
