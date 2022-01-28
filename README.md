# STA-Calc2022
<!DOCTYPE html>
<meta charset="UTF-8">
<html><body>
    <style>
    button
    {
        width: 20px;
        height: 50px;
    }
    </style>
    <input style="font-size: 28px; text-align: right;" /><br />
    <script>
    function update( _v )
    {
        document.quarySelector( 'input' ).value = _v
    }
    
    function append( _v )
    {
        document.quarySelector( 'input' ).value += _v
    }
    
    function cale()
    {
        const v = document.quarySelector( 'input' ).value
        try{
           cont f = new Function( 'return' + v )
           update( f().toString() )
        }catch( _error ){
           update( _error )
        }
    }
    </script>
    <button onclick="append( '1' )" >1</button>
    <button onclick="append( '2' )" >2</button
    <button onclick="append( '3' )" >3</button>
    <button onclick="append( '4' )" >4</button>
    <button onclick="append( '5' )" >5</button>
    <button onclick="append( '6' )" >6</button>
    <button onclick="append( '7' )" >7</button>
    <button onclick="append( '8' )" >8</button>
    <button onclick="append( '9' )" >9</button>
    <button onclick="append( '0' )" >0</button>
    <button onclick="append( '.' )" >.</button>
    <button onclick="append( '+' )" >+</button>
    <button onclick="append( '-' )" >-</button>
    <button onclick="append( '*' )" >*</button>
    <button onclick="append( '/' )" >/</button>
    <button onclick="append( '**' )" >^</button>
    <button onclick="append( '**0.5' )" >√</button>

    <button onclick="cale()" style="width:105px;" >=</button>

    <button onclick="update( '' )" >CLR</button>
</body></html>

  
