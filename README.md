# Roulette-Microbit
抽選などをする際にルーレットを使うときにルーレットの準備のストレスから開放します

コード(Python)
β1.0

def on_button_pressed_ab():
    global シャッフル, Roulette
    シャッフル = randint(1, 50)
    basic.show_string("" + str(シャッフル))
    for index in range(シャッフル):
        Roulette = randint(0, 100)
        basic.show_string("" + str(Roulette))
    if Roulette == 7:
        basic.show_string("OMEDETOU")
    else:
        basic.show_string("ZANNEN")
    if Roulette == 77:
        basic.show_string("OOOMEDETOU")
input.on_button_pressed(Button.AB, on_button_pressed_ab)

Roulette = 0
シャッフル = 0
basic.show_leds("""
    . # # # .
        # . # . #
        # . # # #
        # . . . #
        . # # # .
""")
basic.show_string("Roulette")
basic.pause(100)
basic.show_string("Please A+B")

β1.1

def on_button_pressed_ab():
    global シャッフル, Roulette
    シャッフル = randint(1, 50)
    basic.show_string("" + str(シャッフル))
    for index in range(シャッフル):
        Roulette = randint(0, 100)
        basic.show_string("" + str(Roulette))
    if Roulette == 7:
        basic.show_string("OMEDETOU")
    else:
        basic.show_string("ZANNEN")
    if Roulette == 77:
        basic.show_string("OOOMEDETOU")
    if Roulette == 1:
        basic.show_string("pittarisugoi!!!")
    basic.pause(100)
    basic.show_string("Thank you For Use!")
input.on_button_pressed(Button.AB, on_button_pressed_ab)

Roulette = 0
シャッフル = 0
basic.show_leds("""
    . # # # .
        # . # . #
        # . # # #
        # . . . #
        . # # # .
""")
basic.pause(100)
basic.show_string("Roulette")
basic.pause(100)
basic.show_string("Running To Version b1.1")
basic.pause(100)
basic.show_string("Build 2022724-2")
basic.pause(100)
basic.show_string("Please A+B")
