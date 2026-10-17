# cadastro_usuario
Plataforma de cadastro de usuarios com menu interativo.

    usuarios = []
    
    while True:
    print("\n1 - Cadastrar")
    print("2 - Listar")
    print("3 - Sair")

    opcao = input("Escolha: ")

    if opcao == "1":

        nome = input("Nome: ")
        email = input("Email: ")

        usuario = {
            "nome": nome,
            "email": email
        }

        usuarios.append(usuario)

        print("Usuário cadastrado!")

    elif opcao == "2":

        for usuario in usuarios:
            print(f"Nome: {usuario['nome']}")
            print(f"Email: {usuario['email']}")
            print("-" * 20)

    elif opcao == "3":
        print("Encerrando...")
        break
