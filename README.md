# PiToilet
The project for IoT.
This project is used for monitoring whether the toilet is occupied or not 
It may be utiilized in many factories or assembly lines where employees are working in a very stressed and busy environment
### Written in Python

</IO.setwarnings(False)>
<IO.setmode(IO.BOARD)>

IO.setup(3,IO,OUT)  #GPIO 3 Red Light as output 
IO.setup(5,IO,OUT)  #GPIO 5 Green Light as output
IO.setup(8,IO,IN)  #GPIO 8 IR sesnsor as input

while 1:
 if (IO.input(8)==True):
  print("Object Far")
  IO.(output 3, TRUE)
  IO.(output 5, False)

esle
  print("Object Near")
  IO.(output 5, TRUE)
  IO.(output 3, False)

 time.sleep(1.5)
