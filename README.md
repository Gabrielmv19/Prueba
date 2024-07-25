# Prueba
function manufacture(gifts, materials) {
  const materialList = materials.split('')
  return gifts.filter(gift =>{
    const giftMaterials = gift.split('')
    return giftMaterials.every(materialGift =>
    materialList.includes(materialGift)
    )
  }
  )
  return []
}
