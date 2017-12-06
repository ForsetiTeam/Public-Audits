# ForsetiDev

1. Основа токена описана в файле StandartToken.sol - это стандартный токен ERC20 от openZeppelin
2. Mintable.sol - описана логика выпуска токенов для разных случаев, когда добваляем контракты имеющие права выпускать токены в ручную и когда есть единственный контракт owner  который может минтить токены, в случае если токен создается из контракта краудсейл.
3. Others.sol - содержит классы Ownable, ReentrancyGuard, Statefull.
4. StandartCrowdsale.sol - стандартный краудсейл без дополнительных функций наследуем от него вновь создаваемый контракт краудсейла и добавляем свои кастомные функции, не забываем о контрактах из Others
5. FiatPrice.sol - упрощенный самописный контракт с курсами фиатных валют к эфиру.
