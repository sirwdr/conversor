# conversor
```markdown
# Convertidor a Snake Case

Este proyecto contiene una función en Python que convierte una cadena en formato PascalCase o camelCase a snake_case.

## Código

```python
def convert_to_snake_case(pascal_or_camel_cased_string):
    snake_cased_char_list = [
        '_' + char.lower() if char.isupper()
        else char
        for char in pascal_or_camel_cased_string
    ]
    return ''.join(snake_cased_char_list).strip('_')

def main():
    print(convert_to_snake_case('IAmAPascalCasedString'))

main()
```

## Uso

Para usar la función `convert_to_snake_case`, simplemente llama a la función con una cadena en formato PascalCase o camelCase. Por ejemplo:

```python
print(convert_to_snake_case('IAmAPascalCasedString'))
```

Esto imprimirá:

```
i_am_a_pascal_cased_string
```
