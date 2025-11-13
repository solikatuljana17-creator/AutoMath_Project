# AutoMath_Project
              switch (operation) {
                case '+': result = prev + curr; break;
                case '-': result = prev - curr; break;
                case '*': result = prev * curr; break;
                case '/': 
                    if (curr === 0) {
                        alert('Error: Tidak bisa membagi dengan nol!');
                        clearDisplay();
                        return;
                    }
                    result = prev / curr; 
                    break;
                default: return;
            }
            display.value = result;
            currentInput = result.toString();
            previousInput = '';
            operation = null;
        }
        function clearDisplay() {
            display.value = '';
            currentInput = '';
            previousInput = '';
            operation = null;
        }
    </script>
</body>
</html>


