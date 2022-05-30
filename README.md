p=1
while p!=0:
    menuprincipal=  (print("bienvenido al bufete de abogados, seleccione la opcion necesaria dependiendo que tipo de usuario es usted: [1]cliente [2]abogado [3]representante [4]secretari@ [5]contador [0]salir."))
    
    opcion = int(input ("debes digitar un numero del 1 al 5:"))
    
    if opcion == 1:
        while opcion != 0:
            cliente =int( input ("bienvenido al sistema, acontinuacion ingrese la opcion que desee tomar: [1]tomar una cita [2]cancelar una cita [3]como contratar un abogado [4] ver estado de mi proceso [0]salir:"))
            if cliente == 1:
                tomarcita = input ("ingrese su nombre completo y apellidos: ")
                print ("su nombre es {},".format (tomarcita))
                tomarcita = input ("ingrese su cedula:")
                print ("su cedula es {},".format (tomarcita))
                tomarcita = input ("ingrese su correo electronico:")
                print ("su correo electronico es {},".format (tomarcita))
                tomarcita = input ("sus datos fueron correctamente procesados a continuacion eliga la fecha que mas se acomode a su agenda [1] 11/05/2022 [2] 24/05/2022:")
                if tomarcita ==1:
                    print ("su cita fue agendada correctamente, pronto le llegara un correo electronico de nuestro sistema")
                else:
                    print ("su cita fue agendada correctamente, pronto le llegara un correo electronico de nuestro sistema")
            elif cliente == 2:
                cancelarcita = input ("ingrese su nombre completo y apellidos:")
                print ("su nombre es {}, verificando nombre en el sistema...".format (cancelarcita))
                cancelarcita = input ("ingrese su cedula:")
                print ("su cedula es {}, verificando datos en el sistema...")
                cancelarcita = input ("usted tomo una cita para el dia 24/07/2022, ¿desea cancelarla? [si] [no]:")
                if cancelarcita == "si":
                    print ("su cita fue cancelada correctamente")
                else:
                    print ("su cita sigue agendada en nuestro sistema")
            elif cliente == 3:
                print ("para contratar nuestros servicios debe tener una cedula de ciudadania, en caso de ser menor de edad (7 años en adelante) tener su tarjeta de identidad, un correo electronico real y un domicilio principal en donde podamos ubicarlo. contamos con abogados con conocimientos sobre asuntos penales, laborales, civiles, administrativos y de familia. ")
            elif cliente == 4:
                verestadodemiproceso = input ("ingrese su nombre y apellido:")
                print ("su nombre es {}".format (verestadodemiproceso))
                verestadodemiproceso = input ("ingrese su cedula:")
                print ("su cedula es {}".format (verestadodemiproceso))
                verestadodemiproceso = input ("ingrese el codigo de su caso otorgado por su abogado:")
                print ("validando informacion. recibira un correo de nuestro sistema en donde le brindaremos mayor informacion sobre su proceso")
            else:
                opcion=cliente
    
    elif opcion == "2":
        abogado = int(input ("digite su codigo de abogado:"))
        op1=int(input ("Acontinuacion ingrese la opcion que usted crea necesaria [1]expedientes [2]citas de clientes [3]audiencias:"))
        expediente = input ("usted tiene asignado 2 casos, eliga el expediente necesario [1]Juan Torres codigo 2425 [2]Sofia Vergara codigo 2328:")
        if expediente == "1":
               op2=int( input ("caso 2425, [1]nombre de funcionarios publicos implicados [2]hechos [3]actores y victimas [4]testigos: "))
               if op2 == 1:
                   print ("juez: Leider Arrieta Gomez, secretario: Daniel Gonzalez Reyes, juzgado: juzgado septimo familia cartagena, fiscal: efrain Gonzalez, Defensor general: Kobe bryan ")
               if op2 == 2:
                   print ("el hombre Juan Camilo Torres Molina de 27 años de edad, es acusado de homicidio en primer grado, el hombre se encontraba en la discoteca wakanda al rededor de las 2:00 AM, cuando dos hombres se le acercaron con la intencion de robarlo, el en defensa legitima saco un arma cortopunzante y agredio a uno de los hombres, el cual luego de 21 horas estando en UCI fue declarado muerto")
               if op2 == 3:
                   print ("Actores: Juan Camilo Torres Molina, 27 años de edad, estatura 1.85cm, tez blanca. Victimas: Camilo Andres Fortich, 30 años de edad, estatura 1.75cm, tez morena.")
               if op2 == 4:
                   print ("testigos: Sofia Natalia Giraldo, parentesco amiga. Emilio Andres Torres Molina, parentesco hermano.")
        elif expediente == "2":
               op2=int (input("caso 2328, [1]nombre de funcionarios publicos implicados [2]hechos [3]actores y victimas [4]testigos: "))
               if op2 == 1:
                   print ("juez:Zacarias jose Quesada Gonzalez, secretario: Juan Carlos Jimenez, juzgado: juzgado sexto familia cartagena, fiscal: Sebastian Jose Padilla, defensor general: Edgar David Gomez")
               if op2 == 2:
                   print ("la mujer Sofia Vergara de 38 años de edad, es acusada de hurto a mano armada, los hechos sucedieron el dia 24/02/2022 a las 12:00PM, las camaras de seguridad registraron el momento en donde la denunciada accede al centro comercial y saca de su mochila un arma cortopunzante para robar ")
                
    elif opcion== "3":
        representante  = input ("digite su codigo de representante")
        print ("su codigo es {}".format (representante ))
        input ("bienvenido al sistema a continuacion eliga la opcion que necesite: [1]expedientes [3]pagos [4]nomina de abogados [5]citas [6]reuniones ")
