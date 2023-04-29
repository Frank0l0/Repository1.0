import time

def intro():
    print("Willkommen zu unserem Abenteuerspiel! ")
    time.sleep(2)
    print("Sie wachen in einer Höhle auf und haben keine Ahnung, wie Sie hierher gekommen sind.")
    time.sleep(2)
    print("Ihr Ziel ist es, einen Ausweg zu finden und zu entkommen.")
    time.sleep(2)
    print("Bereit?")

def choose_path():
    print("Sie sehen zwei Wege vor sich.")
    time.sleep(2)
    print("Der linke Pfad führt durch eine enge Felsspalte.")
    time.sleep(2)
    print("Der rechte Pfad führt zu einem dunklen Tunnel.")
    time.sleep(2)
    path = input("Welchen Pfad möchten Sie wählen? (l/r) ")
    if path == "l":
        print("Sie haben den linken Pfad gewählt.")
        time.sleep(2)
        print("Der Pfad wird immer enger und Sie müssen sich durchzwängen.")
        time.sleep(2)
        print("Sie kommen schließlich an eine Sackgasse und müssen umkehren.")
        choose_path()
    elif path == "r":
        print("Sie haben den rechten Pfad gewählt.")
        time.sleep(2)
        print("Der Tunnel ist sehr dunkel und Sie können kaum etwas sehen.")
        time.sleep(2)
        print("Sie hören das Geräusch von Tropfwasser und fühlen sich unwohl.")
        time.sleep(2)
        print("Aber Sie bemerken eine Lichtquelle in der Ferne.")
        time.sleep(2)
        print("Es könnte der Ausgang sein!")
        time.sleep(2)
        print("Sie folgen dem Licht und schließlich finden Sie den Ausgang.")
        time.sleep(2)
        print("Sie haben das Spiel gewonnen!")
    else:
        print("Ungültige Eingabe. Bitte wählen Sie erneut.")
        choose_path()

def play_game():
    intro()
    choose_path()

play_game()
