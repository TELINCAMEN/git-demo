# git-demo

# Definir las notas de la canción (frecuencia en Hz)
$notas = @{
    "Do"  = 261.63
    "Re"  = 293.66
    "Mi"  = 329.63
    "Fa"  = 349.23
    "Sol" = 392.00
    "La"  = 440.00
    "Si"  = 493.88
}

# Reproducir la canción
foreach ($nota in "Do", "Re", "Mi", "Fa", "Sol", "La", "Si", "La", "Sol", "Fa", "Mi", "Re", "Do") {
    $frecuencia = $notas[$nota]
    Write-Host "Reproduciendo nota $nota con frecuencia $frecuencia Hz..."
    [Console]::Beep($frecuencia, 500) # Cada nota dura 0.5 segundos
}


