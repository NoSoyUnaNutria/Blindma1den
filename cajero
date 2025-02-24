user_r = 'blindma1den'
pswd_r = '1234'
user2_tf = 'nutr1a'
intentos = 3

saldo = 2000

while intentos > 0:
    user = input('Ingresa el nombre de usuario: ')
    pswd = input('Ingresa la contraseña: ')
    if user == user_r and pswd == pswd_r:
        print('Acceso concedido.')
        break
    else:
        intentos -= 1
        print(f'Los datos ingresados no son correctos. te quedan {intentos} intentos.')
if intentos == 0:
    print('Usuario Bloqueado.')
    exit(0)

print('----------------------------------------------------')
print('Bienvenido.')
print(f'Su saldo es de: {saldo}'+'$')
print('(A) Depositar')
print('(B) Retirar')
print('(C) Transferir')
print('(D) Salir')

while True:
    print('----------------------------------------------------')
    opcion = input('Selecione la accion a realizar: ')
    if opcion == 'A' or opcion == 'a' or opcion == 'depositar' or opcion =='Depositar' or opcion == 'DEPOSITAR':
        try:
            deposito = input('Ingresa el monto que deseas depositar: ')
            saldo += float(deposito)
            print(f'Su deposito de ${deposito} se a realizado exitosamente.')
            print(f'Su saldo actual es de ${saldo}')    
            
        except ValueError:
            print('Por favor, ingrese un numero valido.')
    elif opcion == 'B' or opcion == 'b' or opcion == 'Retirar' or opcion == 'retirar' or opcion == 'RETIRAR':
        retiro = ''
        try:
            retiro = input('Ingrese el monto que desea retirar: ')
            if saldo < float(retiro):
                print('Saldo insuficiente.')
            else:
                saldo -= float(retiro)
                print(f'Su retiro de ${float(retiro)} se a realizado exitosamente.')
                print(f'Su saldo actual es de ${saldo}')
                
        except ValueError:
            print('Por favor, ingrese un numero valido.')
            
    elif opcion == 'C' or opcion == 'c' or opcion == 'Transferir' or opcion == 'transferir' or opcion == 'TRASFERIR':
        transferir = ''
        
        try:
            transferir = input('Ingrese el monto que de sea transferir: ')
            user_tf = input('Ingrese el nombre del usuario a quien desea transferir: ')
            if saldo < float(transferir):
                print('Saldo insuficiente.')
            elif user_tf != user2_tf:
                print('El usuario no existe. Verifica el usuario.')
            else:
                saldo -= float(transferir)
                print(f'Su transferencia de ${float(transferir)} se a realizado exitosamente.')
                print(f'Su saldo actual es de ${saldo}')
                
        except ValueError:
            print('Por favor, ingrese un numero valido.')
    elif opcion == 'Salir' or opcion == 'salir' or opcion == 'SALIR' or opcion == 'd' or opcion == 'D':
        print('Fue un placer tenerte por aca. Vuelve pronto.')
        break
