# Eliminar ceros a la izquierda de number_format PHP

```php
function clean_num( $num ){
  $pos = strpos($num, '.');

  if($pos === false) { 
    // it is integer number
    return $num;
  }
  else{
    // it is decimal number
    return rtrim(rtrim($num, '0'), '.');
  }
}
```
