# micronaut.inject Skill

Use this skill to work with Norm module `micronaut.inject` version 12. Use only declarations listed below.

## `micronaut.inject`

Source: `JavaArrays.norm`

### `JavaStringArray`

```norm
class JavaStringArray
```

#### `JavaStringArray`

```norm
JavaStringArray(JavaStringArrayBindingToken token)
```

Parameters:

- `token`: `JavaStringArrayBindingToken`

#### `size`

```norm
Integer size()
```

Returns: `Integer`

#### `get`

```norm
String? get(Integer index)
```

Parameters:

- `index`: `Integer`

Returns: `String?`

#### `set`

```norm
Void set(Integer index, String? value)
```

Parameters:

- `index`: `Integer`
- `value`: `String?`

Returns: `Void`

### `javaStringArrayNew`

```norm
JavaStringArray javaStringArrayNew(Integer size)
```

Parameters:

- `size`: `Integer`

Returns: `JavaStringArray`

### `JavaClassArray`

```norm
class JavaClassArray
```

#### `JavaClassArray`

```norm
JavaClassArray(JavaClassArrayBindingToken token)
```

Parameters:

- `token`: `JavaClassArrayBindingToken`

#### `size`

```norm
Integer size()
```

Returns: `Integer`

#### `get`

```norm
Class<?>? get(Integer index)
```

Parameters:

- `index`: `Integer`

Returns: `Class<?>?`

#### `set`

```norm
Void set(Integer index, Class<?>? value)
```

Parameters:

- `index`: `Integer`
- `value`: `Class<?>?`

Returns: `Void`

### `javaClassArrayNew`

```norm
JavaClassArray javaClassArrayNew(Integer size)
```

Parameters:

- `size`: `Integer`

Returns: `JavaClassArray`

## `micronaut.inject.context`

Source: `context/ApplicationContext.norm`

### `ApplicationContext`

```norm
interface ApplicationContext extends BeanContext, PropertyResolver, PropertyPlaceholderResolver
```

#### `close`

```norm
Void close()
```

Returns: `Void`

### `applicationContextRun`

```norm
ApplicationContext? applicationContextRun()
```

Returns: `ApplicationContext?`

### `applicationContextRun`

```norm
T? applicationContextRun<T extends AutoCloseable>(Class<T>? arg0, JavaMap<String, Any>? arg1, JavaStringArray? arg2)
```

Type parameters:

- `T` extends `AutoCloseable`

Parameters:

- `arg0`: `Class<T>?`
- `arg1`: `JavaMap<String, Any>?`
- `arg2`: `JavaStringArray?`

Returns: `T?`

### `applicationContextRun`

```norm
T? applicationContextRun<T extends AutoCloseable>(Class<T>? arg0, JavaStringArray? arg1)
```

Type parameters:

- `T` extends `AutoCloseable`

Parameters:

- `arg0`: `Class<T>?`
- `arg1`: `JavaStringArray?`

Returns: `T?`

### `applicationContextRun`

```norm
ApplicationContext? applicationContextRun(JavaMap<String, Any>? arg0, JavaStringArray? arg1)
```

Parameters:

- `arg0`: `JavaMap<String, Any>?`
- `arg1`: `JavaStringArray?`

Returns: `ApplicationContext?`

## `micronaut.inject.context`

Source: `context/BeanContext.norm`

### `BeanContext`

```norm
interface BeanContext extends LifeCycle<BeanContext>, ExecutionHandleLocator, BeanLocator, BeanDefinitionRegistry, ApplicationEventPublisher<Any>, AnnotationMetadataResolver, MutableAttributeHolder, ConversionServiceProvider
```

#### `close`

```norm
Void close()
```

Returns: `Void`

#### `inject`

```norm
T? inject<T>(T? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `T?`

Returns: `T?`

## `micronaut.inject.context`

Source: `context/BeanDefinitionRegistry.norm`

### `BeanDefinitionRegistry`

```norm
interface BeanDefinitionRegistry
```

## `micronaut.inject.context`

Source: `context/BeanLocator.norm`

### `BeanLocator`

```norm
interface BeanLocator
```

#### `getBean`

```norm
T? getBean<T>(Class<T>? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `Class<T>?`

Returns: `T?`

## `micronaut.inject.context`

Source: `context/ExecutionHandleLocator.norm`

### `ExecutionHandleLocator`

```norm
interface ExecutionHandleLocator
```

## `micronaut.inject.context`

Source: `context/LifeCycle.norm`

### `LifeCycle`

```norm
interface LifeCycle<T extends LifeCycle<T>> extends Closeable, AutoCloseable
```

Type parameters:

- `T` extends `LifeCycle<T>`

#### `close`

```norm
Void close()
```

Returns: `Void`

## `micronaut.inject.context.annotation`

Source: `context/annotation/AliasFor.norm`

### `AliasFor`

```norm
annotation AliasFor implements FunctionTarget, RuntimeRetention, RepeatableAnnotation
```

#### `annotation`

```norm
Class<?> annotation
```

Type: `Class<?>`

#### `annotationName`

```norm
String annotationName
```

Type: `String`

#### `member`

```norm
String member
```

Type: `String`

#### `AliasFor`

```norm
AliasFor(Class<?>? annotation, String? annotationName, String? member)
```

Parameters:

- `annotation`: `Class<?>?`
- `annotationName`: `String?`
- `member`: `String?`

## `micronaut.inject.context.annotation`

Source: `context/annotation/Bean.norm`

### `Bean`

```norm
annotation Bean implements TypeTarget, FieldTarget, FunctionTarget, RuntimeRetention
```

#### `preDestroy`

```norm
String preDestroy
```

Type: `String`

#### `typed`

```norm
List<Class<?>> typed
```

Type: `List<Class<?>>`

#### `Bean`

```norm
Bean(String? preDestroy, List<Class<?>>? typed)
```

Parameters:

- `preDestroy`: `String?`
- `typed`: `List<Class<?>>?`

## `micronaut.inject.context.annotation`

Source: `context/annotation/ConfigurationInject.norm`

### `ConfigurationInject`

```norm
annotation ConfigurationInject implements ConstructorTarget, FunctionTarget, RuntimeRetention
```

#### `value`

```norm
String value
```

Type: `String`

#### `ConfigurationInject`

```norm
ConfigurationInject(String? value)
```

Parameters:

- `value`: `String?`

## `micronaut.inject.context.annotation`

Source: `context/annotation/ConfigurationProperties.norm`

### `ConfigurationProperties`

```norm
annotation ConfigurationProperties implements TypeTarget, ConstructorTarget, FunctionTarget, RuntimeRetention
```

#### `cliPrefix`

```norm
List<String> cliPrefix
```

Type: `List<String>`

#### `excludes`

```norm
List<String> excludes
```

Type: `List<String>`

#### `includes`

```norm
List<String> includes
```

Type: `List<String>`

#### `value`

```norm
String value
```

Type: `String`

#### `ConfigurationProperties`

```norm
ConfigurationProperties(List<String>? cliPrefix, List<String>? excludes, List<String>? includes, String value)
```

Parameters:

- `cliPrefix`: `List<String>?`
- `excludes`: `List<String>?`
- `includes`: `List<String>?`
- `value`: `String`

## `micronaut.inject.context.annotation`

Source: `context/annotation/Context.norm`

### `Context`

```norm
annotation Context implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

Source: `context/annotation/EachProperty.norm`

### `EachProperty`

```norm
annotation EachProperty implements TypeTarget, FunctionTarget, RuntimeRetention
```

#### `excludes`

```norm
List<String> excludes
```

Type: `List<String>`

#### `includes`

```norm
List<String> includes
```

Type: `List<String>`

#### `list`

```norm
Boolean list
```

Type: `Boolean`

#### `primary`

```norm
String primary
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `EachProperty`

```norm
EachProperty(List<String>? excludes, List<String>? includes, Boolean? list, String? primary, String value)
```

Parameters:

- `excludes`: `List<String>?`
- `includes`: `List<String>?`
- `list`: `Boolean?`
- `primary`: `String?`
- `value`: `String`

## `micronaut.inject.context.annotation`

Source: `context/annotation/Executable.norm`

### `Executable`

```norm
annotation Executable implements TypeTarget, FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `processOnStartup`

```norm
Boolean processOnStartup
```

Type: `Boolean`

#### `Executable`

```norm
Executable(Boolean? processOnStartup)
```

Parameters:

- `processOnStartup`: `Boolean?`

## `micronaut.inject.context.annotation`

Source: `context/annotation/Factory.norm`

### `Factory`

```norm
annotation Factory implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

Source: `context/annotation/Primary.norm`

### `Primary`

```norm
annotation Primary implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

Source: `context/annotation/Property.norm`

### `Property`

```norm
annotation Property implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention, RepeatableAnnotation
```

#### `defaultValue`

```norm
String defaultValue
```

Type: `String`

#### `name`

```norm
String name
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `Property`

```norm
Property(String? defaultValue, String name, String? value)
```

Parameters:

- `defaultValue`: `String?`
- `name`: `String`
- `value`: `String?`

## `micronaut.inject.context.annotation`

Source: `context/annotation/Prototype.norm`

### `Prototype`

```norm
annotation Prototype implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

Source: `context/annotation/Replaces.norm`

### `Replaces`

```norm
annotation Replaces implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

#### `named`

```norm
String named
```

Type: `String`

#### `value`

```norm
Class<?> value
```

Type: `Class<?>`

#### `Replaces`

```norm
Replaces(String? named, Class<?>? value)
```

Parameters:

- `named`: `String?`
- `value`: `Class<?>?`

## `micronaut.inject.context.annotation`

Source: `context/annotation/Requires.norm`

### `Requires`

```norm
annotation Requires implements PackageTarget, TypeTarget, FieldTarget, FunctionTarget, RuntimeRetention, RepeatableAnnotation
```

#### `beans`

```norm
List<Class<?>> beans
```

Type: `List<Class<?>>`

#### `missing`

```norm
List<Class<?>> missing
```

Type: `List<Class<?>>`

#### `notEquals`

```norm
String notEquals
```

Type: `String`

#### `property`

```norm
String property
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `Requires`

```norm
Requires(List<Class<?>>? beans, List<Class<?>>? missing, String? notEquals, String? property, String? value)
```

Parameters:

- `beans`: `List<Class<?>>?`
- `missing`: `List<Class<?>>?`
- `notEquals`: `String?`
- `property`: `String?`
- `value`: `String?`

## `micronaut.inject.context.annotation`

Source: `context/annotation/Secondary.norm`

### `Secondary`

```norm
annotation Secondary implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

## `micronaut.inject.context.annotation`

Source: `context/annotation/Type.norm`

### `Type`

```norm
annotation Type implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention
```

#### `value`

```norm
List<Class<?>> value
```

Type: `List<Class<?>>`

## `micronaut.inject.context.annotation`

Source: `context/annotation/Value.norm`

### `Value`

```norm
annotation Value implements TypeTarget, FieldTarget, FunctionTarget, ParameterTarget, RuntimeRetention
```

#### `value`

```norm
String value
```

Type: `String`

## `micronaut.inject.context.env`

Source: `context/env/PropertyPlaceholderResolver.norm`

### `PropertyPlaceholderResolver`

```norm
interface PropertyPlaceholderResolver
```

## `micronaut.inject.context.event`

Source: `context/event/ApplicationEventPublisher.norm`

### `ApplicationEventPublisher`

```norm
interface ApplicationEventPublisher<T>
```

Type parameters:

- `T`

## `micronaut.inject.core.annotation`

Source: `core/annotation/AnnotationMetadataResolver.norm`

### `AnnotationMetadataResolver`

```norm
interface AnnotationMetadataResolver
```

## `micronaut.inject.core.attr`

Source: `core/attr/AttributeHolder.norm`

### `AttributeHolder`

```norm
interface AttributeHolder
```

## `micronaut.inject.core.attr`

Source: `core/attr/MutableAttributeHolder.norm`

### `MutableAttributeHolder`

```norm
interface MutableAttributeHolder extends AttributeHolder
```

## `micronaut.inject.core.convert`

Source: `core/convert/ConversionServiceProvider.norm`

### `ConversionServiceProvider`

```norm
interface ConversionServiceProvider
```

## `micronaut.inject.core.value`

Source: `core/value/PropertyResolver.norm`

### `PropertyResolver`

```norm
interface PropertyResolver extends ValueResolver<String>
```

## `micronaut.inject.core.value`

Source: `core/value/ValueResolver.norm`

### `ValueResolver`

```norm
interface ValueResolver<K extends CharSequence>
```

Type parameters:

- `K` extends `CharSequence`

