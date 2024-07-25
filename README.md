# Prueba
function manufacture(gifts, materials) { /*Crear la función de listado de materiales*/ 
  const materialList = materials.split('') /*Tomo todos los valores de los materiales y lo separo por cada caracter
  generando asi un array o un parameto de cada material*/
  return gifts.filter(gift =>{ /*Filtro lo que son los gifts*/
    const giftMaterials = gift.split('') 
    return giftMaterials.every(materialGift => /*Lo mando a retornar con la condicion que si o si debe tener todos os materiales en la lista*/
    materialList.includes(materialGift)
    )
  }
  )
  return []
}
