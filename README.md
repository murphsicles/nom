# @parsing/nom — Parser Combinators for Zeta

Auto-converted from [nom](https://crates.io/crates/nom) v8.0.0 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
| Category | Combinators |
|----------|-------------|
| **Basic** | tag, take, recognize, consume, eof, success, failure |
| **Sequencing** | preceded, terminated, delimited, separated_pair, tuple |
| **Choice** | alt, permutation |
| **Repetition** | many0, many1, many_m_n, separated_list0, separated_list1, count |
| **Numeric** | i8/i16/i32/i64/u8/u16/u32/u64, f32, f64, hex_u32 |
| **Bytes** | take_while, take_until, is_not, is_a, escaped |
| **Combinators** | map, map_res, map_opt, value, verify, opt, cond, peek, not |
| **Error** | ContextError, ParseError, VerboseError, convert_error |

## Usage
```zeta
use @parsing/nom::*;

fn parse_hex(input: &str) -> IResult<&str, u32> {
    preceded(tag("0x"), hex_u32)(input)
}
```

## Stats: ~13,287 lines across 28 source files, 0 unsupported items

## License
MIT