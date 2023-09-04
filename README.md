# parcial
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurante JR</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1 class="text-center">Restaurante S cocina</h1>
        <form action="pedido.php" method="post">
            <!-- Datos del Cliente -->
            <div class="mb-3">
                <label for="nombre" class="form-label">Nombre:</label>
                <input type="text" class="form-control" id="nombre" name="nombre" required>
            </div>
            <div class="mb-3">
                <label for="direccion" class="form-label">Dirección:</label>
                <input type="text" class="form-control" id="direccion" name="direccion" required>
            </div>
            <div class="mb-3">
                <label for="telefono" class="form-label">Teléfono:</label>
                <input type="tel" class="form-control" id="telefono" name="telefono" required>
            </div>

            <!-- Menú -->
            <h2>Menú</h2>

            <!-- Corrientazo de Pollo -->
            <div class="mb-3">
                <label for="corrientazo_pollo" class="form-label">Corrientazo de Pollo ($10,000 pesos):</label>
                <input type="number" class="form-control" id="corrientazo_pollo" name="corrientazo_pollo" min="0">
            </div>
            
            <!-- Corrientazo de Cerdo -->
            <div class="mb-3">
                <label for="corrientazo_cerdo" class="form-label">Corrientazo de Cerdo ($12,000 pesos):</label>
                <input type="number" class="form-control" id="corrientazo_cerdo" name="corrientazo_cerdo" min="0">
            </div>

            <!-- Corrientazo de Lomo -->
            <div class="mb-3">
                <label for="corrientazo_lomo" class="form-label">Corrientazo de Lomo ($15,000 pesos):</label>
                <input type="number" class="form-control" id="corrientazo_lomo" name="corrientazo_lomo" min="0">
            </div>

            <!-- Sopa -->
            <div class="mb-3">
                <label for="sopa" class="form-label">Sopa ($5,000 pesos):</label>
                <select class="form-select" id="sopa" name="sopa">
                    <option value="costilla"></option>
                    <option value="costilla">Costilla</option>
                    <option value="mondongo">Mondongo</option>
                    <option value="mote_queso">Mote de Queso</option>
                    <option value="mote_queso">Mote de ñame</option>
                    <option value="mote_queso">pollo</option>
                </select>
            </div>

            <!-- Jugo -->
            <div class="mb-3">
                <label for="jugo" class="form-label">Jugo ($2,000 pesos):</label>
                <select class="form-select" id="jugo" name="jugo">
                    <option value="costilla"></option>
                    <option value="maracuya">Maracuyá en agua</option>
                    <option value="maracuya_leche">Maracuyá en leche</option>
                    <option value="fresa">Fresa en agua</option>
                    <option value="fresa_leche">Fresa en leche</option>
                    <option value="mora">Mora en agua</option>
                    <option value="mora_leche">Mora en leche</option>
                </select>
            </div>

            <!-- Gaseosa -->
            <div class="mb-3">
                <label for="gaseosa" class="form-label">Gaseosa ($2,500 pesos):</label>
                <select class="form-select" id="gaseosa" name="gaseosa">
                    <option value="costilla"></option>
                    <option value="coca_cola">Coca-Cola</option>
                    <option value="manzana">Manzana</option>
                    <option value="sprite">Sprite</option>
                    <option value="sprite">cola</option>
                </select>
            </div>

            <!-- Helado -->
            <div class="mb-3">
                <label for="helado" class="form-label">Helado ($3,000 pesos):</label>
                <select class="form-select" id="helado" name="helado">
                    <option value="costilla"></option>
                    <option value="vainilla">Vainilla</option>
                    <option value="chocolate">Chocolate</option>
                    <option value="fresa">Fresa</option>
                    <option value="fresa">frutos rojos</option>
                </select>
            </div>

            <button type="submit" class="btn btn-primary">Hacer pedido</button>
        </form>

        <!-- Factura oculta inicialmente -->
        <div id="factura" class="factura-container">
            <!-- La factura se mostrará aquí después de enviar el formulario -->
        </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.min.js"></script>
    <script src="script.js"></script>
</body>
</html>
