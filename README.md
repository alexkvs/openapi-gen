# openapi-generator-cli-usage

The batch file for generating code from JSON schema files.<br />
Includes options for adding validation annotations to generated GTO's.


See: <br />
OpenAPITools https://github.com/OpenAPITools/openapi-generator-cli <br />
Config Options for Spring https://openapi-generator.tech/docs/generators/spring/


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
