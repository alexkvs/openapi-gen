# openapi-gen-usage

The batch file to generate code from JSON schema files.
Includes options for adding validation annotations to generated GTO's.

Config Options for Spring:
https://openapi-generator.tech/docs/generators/spring/


##### To suppress serializing properties with null values (using Jackson >2.0), you can anntotate generated DTO class with @JsonInclude.

Example:<br />
@JsonInclude(value=JsonInclude.Include.NON_NULL)<br />
public class YouGenareatedDto {
}


##### Annotation that can be used to ignore processing of JSON properties read (during deserialization).

Example:<br />
@JsonIgnoreProperties(ignoreUnknown = true)<br />
public class YouGenareatedDto {
}
