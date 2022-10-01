# projeto-Musicas
nput.onButtonPressed(Button.A, function () {
    music.startMelody(music.builtInMelody(Melodies.Wedding), MelodyOptions.Once)
    basic.showIcon(IconNames.Heart)
})
input.onGesture(Gesture.Shake, function () {
    music.startMelody(music.builtInMelody(Melodies.Dadadadum), MelodyOptions.Once)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
    basic.showIcon(IconNames.Pitchfork)
})
input.onButtonPressed(Button.AB, function () {
    basic.clearScreen()
})
input.onButtonPressed(Button.B, function () {
    basic.showString("" + (input.temperature()))
})
music.playMelody("C5 G D F A C B E ", 120)
basic.forever(function () {
	
})


