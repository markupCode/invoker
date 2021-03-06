# A Dependency-Injection container for mortals

![Pub Version](https://img.shields.io/pub/v/invoker?color=%23004156)
[![CodeFactor](https://www.codefactor.io/repository/github/markupcode/invoker/badge)](https://www.codefactor.io/repository/github/markupcode/invoker)
![GitHub](https://img.shields.io/github/license/markupcode/invoker?color=%2348CFAF)

Attention **Performance Hunters** - creeping types registration, resolution and Mirrors inside!

Has strict dependency on [Dartz](https://github.com/spebbe/dartz)!

## API Draft

### Empty container

```dart
final contianer = ContainerFactory.empty();
```

### Dependency registration

```dart
container.bindWithContract<Weapon, Katana>().asTransient()
         .bindWithContract<Warrior, Ninja>().asTransient();
```

### Dependency resolving

```dart
final warrior = container.resolve<Warrior>();
```
