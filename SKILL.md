# micronaut.inject Skill

Use this skill to work with Norm module `micronaut.inject` version 6. Use only declarations listed below.

## `micronaut.inject.context`

### `ApplicationContext`

```norm
interface ApplicationContext extends BeanContext, PropertyResolver, PropertyPlaceholderResolver
```

#### `close`

```norm
Void close()
```

### `applicationContextRun`

```norm
ApplicationContext? applicationContextRun()
```

### `applicationContextRun`

```norm
T? applicationContextRun<T extends AutoCloseable>(Class<T>? arg0, JavaMap<String, Any>? arg1, JavaStringArray? arg2)
```

### `applicationContextRun`

```norm
T? applicationContextRun<T extends AutoCloseable>(Class<T>? arg0, JavaStringArray? arg1)
```

### `applicationContextRun`

```norm
ApplicationContext? applicationContextRun(JavaMap<String, Any>? arg0, JavaStringArray? arg1)
```

## `micronaut.inject.context`

### `BeanContext`

```norm
interface BeanContext extends LifeCycle<BeanContext>, ExecutionHandleLocator, BeanLocator, BeanDefinitionRegistry, ApplicationEventPublisher<Any>, AnnotationMetadataResolver, MutableAttributeHolder, ConversionServiceProvider
```

#### `close`

```norm
Void close()
```

#### `inject`

```norm
T? inject<T>(T? arg0)
```

## `micronaut.inject.context`

### `BeanLocator`

```norm
interface BeanLocator
```

#### `getBean`

```norm
T? getBean<T>(Class<T>? arg0)
```

## `micronaut.inject.context.annotation`

### `Bean`

```norm
annotation Bean implements TypeTarget, FieldTarget, FunctionTarget, RuntimeRetention
```

#### `preDestroy`

```norm
String preDestroy
```

#### `typed`

```norm
List<Class<?>> typed
```

#### `Bean`

```norm
Bean(String? preDestroy, List<Class<?>>? typed)
```

## `micronaut.inject.context.annotation`

### `ConfigurationInject`

```norm
annotation ConfigurationInject implements ConstructorTarget, FunctionTarget, RuntimeRetention
```

#### `value`

```norm
String value
```

#### `ConfigurationInject`

```norm
ConfigurationInject(String? value)
```

## `micronaut.inject.context.annotation`

### `ConfigurationProperties`

```norm
annotation ConfigurationProperties implements TypeTarget, ConstructorTarget, FunctionTarget, RuntimeRetention
```

#### `cliPrefix`

```norm
List<String> cliPrefix
```

#### `excludes`

```norm
List<String> excludes
```

#### `includes`

```norm
List<String> includes
```

#### `value`

```norm
String value
```

#### `ConfigurationProperties`

```norm
ConfigurationProperties(List<String>? cliPrefix, List<String>? excludes, List<String>? includes, String value)
```

## `micronaut.inject.context.annotation`

### `Context`

```norm
annotation Context implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

### `EachProperty`

```norm
annotation EachProperty implements TypeTarget, FunctionTarget, RuntimeRetention
```

#### `excludes`

```norm
List<String> excludes
```

#### `includes`

```norm
List<String> includes
```

#### `list`

```norm
Boolean list
```

#### `primary`

```norm
String primary
```

#### `value`

```norm
String value
```

#### `EachProperty`

```norm
EachProperty(List<String>? excludes, List<String>? includes, Boolean? list, String? primary, String value)
```

## `micronaut.inject.context.annotation`

### `Executable`

```norm
annotation Executable implements TypeTarget, FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `processOnStartup`

```norm
Boolean processOnStartup
```

#### `Executable`

```norm
Executable(Boolean? processOnStartup)
```

## `micronaut.inject.context.annotation`

### `Factory`

```norm
annotation Factory implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

### `Primary`

```norm
annotation Primary implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

### `Property`

```norm
annotation Property implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention, RepeatableAnnotation
```

#### `defaultValue`

```norm
String defaultValue
```

#### `name`

```norm
String name
```

#### `value`

```norm
String value
```

#### `Property`

```norm
Property(String? defaultValue, String name, String? value)
```

## `micronaut.inject.context.annotation`

### `Prototype`

```norm
annotation Prototype implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

### `Replaces`

```norm
annotation Replaces implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

#### `named`

```norm
String named
```

#### `value`

```norm
Class<?> value
```

#### `Replaces`

```norm
Replaces(String? named, Class<?>? value)
```

## `micronaut.inject.context.annotation`

### `Requires`

```norm
annotation Requires implements PackageTarget, TypeTarget, FieldTarget, FunctionTarget, RuntimeRetention, RepeatableAnnotation
```

#### `beans`

```norm
List<Class<?>> beans
```

#### `missing`

```norm
List<Class<?>> missing
```

#### `notEquals`

```norm
String notEquals
```

#### `property`

```norm
String property
```

#### `value`

```norm
String value
```

#### `Requires`

```norm
Requires(List<Class<?>>? beans, List<Class<?>>? missing, String? notEquals, String? property, String? value)
```

## `micronaut.inject.context.annotation`

### `Secondary`

```norm
annotation Secondary implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

### `Value`

```norm
annotation Value implements TypeTarget, FieldTarget, FunctionTarget, ParameterTarget, RuntimeRetention
```

#### `value`

```norm
String value
```

