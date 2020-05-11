computing_ch3_notes_exercises.md

***Notes***

Compiled programs are faster => translation happens while program is running so interpreter is slower

Compile programs show error


***Exercises**
Exercise 3.4 is super-extra

Exercise 3.4:

Unstated but possibly related:
Distance = Rate * Time
1 Meter = ~39.37 inches

Stated:
Light Travels at 299,792,458 meters per second

Processor Speed is gigahertz (GHz), 1,000,000,000 hertz
  Herts means once per second, so 1 GHz means the processor executes 1,000,000,000 cycles per second

  My machine has a processor has a speed of 1.8 GHz
    1,800,000,000 cycles per second

  In inches, how far does light travel during the time it takes the processor in my computers to execute one cycle.
    1,800,000,000 cycles per second
    299,792,458 meters per second

    Convert speed of light from meters to inches:
      Converting the speed of light from meters to inches:
        ~11,802,852,677.17 Light Speed in Inches Per Second

       If my computer completes 1,800,000,000 cycles per second and light travels at 118,101,829,071.46 inches per second, how far does light travel - in inches - in the time it takes my computers to complete one cycle?

       I'm assuming the computational time is linear; that we we can figure out the fraction of a second it takes to complete one cycle from the 1.8GHz speed -  1,800,000,000 cycles per second

       If 1,800,000,000/1 = 1/x, then:
       (x)1,800,000,000 = 1
       the time it takes to complete one cycle is 1/1,800,000,000

       If light travels at 11,802,852,677.17 inches per second and my computer process one cycle in 1/1,800,000,000, then
       then light will travel inches 11,802,852,677.17*1/1,800,000,000 in the time it takes my computer to complete on cycle.

       11,802,852,677.17*1/1,800,000,000 = ~6.55 inches

       DANG! OK, the scheme representation
       (* 11,802,852,677.17 (/ 1 1800000000))

      Scheme representation, including the conversion from meter to inches
      (* (* 299792458 39.37008) (/ 1 1800000000))

299792458 39.37008
118,102,069,054.85664
 11,802,852,677.17


Exercise 3.5:
  (define (cube x) (* x (* x x)))


