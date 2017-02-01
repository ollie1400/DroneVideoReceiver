# DroneVideoReceiver

A circuit board for a receiver module of a 5.8GHz video signal.  The main receiver component is the RX5808.  The board is mainly just supporting components for the RX5808 and doesn't do much.

A DC power jack passes via a toggle switch, and then through a voltage regulator.  This supplies the RX5808 with 5V.  The supply is decoupled by a 470uF electrolytic capacitor.  An LED is used to indicate power.

The CH1, CH2 and CH3 pins can be tied to ground by placing jumpers on J1.  e.g. To ground CH1 one would place a jumper between pins 1 and 2 of J1.
RSSI and Audio output from the RX5808 are taken straight to pins 1 and 2 on J3, as well as test points on the board.
Video output is taken through capacitor C2 to pin 3 on J3, and a test point.

The antenna port is taken to a planar SMA connector on the board.  The signal trace and surrounding traces have been designed to present 50Ohm impedance.

# Components

| Marker | Name                   | Quantity |
|--------|------------------------|----------|
| C1, C2 | 470uF Capacitor        | 2        |
| D1     | LED                    | 1        |
| J1     | 6 pin header           | 1        |
| J3     | 3 pin header           | 1        |
| R1     |  1K Resistor           | 1        |
| U1     | L7805CV                | 1        |
| U2     | DCJack2.1mm            | 1        |
| U3     | RX5808                 | 1        |
| U4     | SMA connector (female) | 1        |
| U32    | SPswitch               | 1        |
