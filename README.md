# Roulette-Microbit
抽選などをする際にルーレットを使うときにルーレットの準備のストレスから開放します

利用規約
完全オープンソースなので
自作発言以外だったらどんなことに使ってもいいです

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

Release 1.0


Roulette = 0
シャッフル = 0
basic.show_leds("""
    . # # # .
        # # . # #
        # . # . #
        # # . # #
        . # # # .
""")
basic.pause(100)
basic.show_string(" Roulette-micro:bit")
basic.pause(10)
basic.show_string("Running To Version Release-v1.0")
basic.pause(10)
basic.show_string("Thank you for downloads!")
basic.pause(10)
basic.show_string("Build 2022725")
basic.pause(10)
basic.show_string("©2022 yuki110319")
basic.pause(10)
basic.show_string("Please A+B or A or B")

def on_forever():
    global シャッフル, Roulette
    if input.button_is_pressed(Button.B):
        basic.show_string("OK Roulette Start")
        シャッフル = randint(1, 100)
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
basic.forever(on_forever)

def on_forever2():
    global シャッフル, Roulette
    if input.button_is_pressed(Button.A):
        basic.show_string("OK Roulette Start")
        シャッフル = randint(1, 10)
        basic.show_string("" + str(シャッフル))
        for index2 in range(シャッフル):
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
basic.forever(on_forever2)

def on_forever3():
    global シャッフル, Roulette
    if input.button_is_pressed(Button.AB):
        basic.show_string("OK Roulette Start")
        シャッフル = randint(1, 50)
        basic.show_string("" + str(シャッフル))
        for index3 in range(シャッフル):
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
basic.forever(on_forever3)
