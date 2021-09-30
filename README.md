# openapi-gen

Config Options for Spring:
https://openapi-generator.tech/docs/generators/spring/


To suppress serializing properties with null values (using Jackson >2.0), you can anntotate generated DTO class with @JsonInclude
For example:

@JsonInclude(value=JsonInclude.Include.NON_NULL)
public class YouGenareatedDto {
}
