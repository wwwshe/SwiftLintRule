# SwiftLintRule

Default 룰
blanket_disable_command: Swiftlint:disable 명령은 파일이 끝나기 전에 다시 활성화 규칙
block_based_kvo: Swift 3.2 이상을 사용할 때 키 경로가 포함된 새로운 블록 기반 KVO API를 선호 규칙
class_delegate_protocol: 위임 프로토콜은 약하게 참조될 수 있도록 클래스 전용 규칙
closing_brace: 닫는 괄호가 있는 닫는 중괄호는 중간에 공백이 없어야 하는 규칙
closure_parameter_position: 클로저 매개변수는 여는 중괄호와 같은 줄에 있어야 하는 규칙
colon: 유형을 지정할 때는 식별자 옆에, 사전 리터럴에서는 키 옆에 콜론이 있어야 하는 규칙
comma: 쉼표 앞이나 뒤에는 공백이 없어야 하는 규칙
comment_spacing: 주석 슬래시 뒤에 공백이 한개 이상이 있어야 하는 규칙
compiler_protocol_init: 컴파일러 프로토콜에서 선언된 초기화 프로그램은 ExpressibleByArrayLiteral을 직접 호출하면 안 되는 규칙
computed_accessors_order: Getter와 Setter는 get set 순서로 되어하는 규칙
control_statement: if, for, guard, switch, while 및 catch문은 조건문이나 인수를 괄호 안에 불필요하게 묶어서는 안 되는 규칙
cyclomatic_complexity: 함수 본문의 복잡성 제한규칙(10이상 경고 20이상은 에러)
deployment_target: 가용성 검사 또는 속성은 배포 대상이 충족하는 이전 버전을 사용해서는 안 되는 규칙
discouraged_direct_init: 권장되지 않는 직접 초기화규칙 ex) Bundle(), UIDevice() 등등
duplicate_conditions: 중복된 조건 체크 규칙
duplicate_enum_cases: Enum case 중복 체크 규칙
duplicate_imports: import 중복 체크 규칙
duplicated_key_in_dictionary_literal: Dictionary 중복 키 체크 규칙
dynamic_inline: 'dynamic'과 '@inline(__always)'을 같이 쓰면 안 되는 규칙
empty_enum_arguments: Enum case 인수가 사용되지 않을때 생략 규칙 ex) case .bar(_) -> case .bar()
empty_parameters: 빈 파라메터를 표시할 때 () 보단 Void를 선호하는 규칙
empty_parentheses_with_trailing_closure: 후행 클로저를 사용할 때 메소드 호출 후에 빈 괄호를 생략 규칙
file_length: 파일 라인수 체크 규칙
for_where: for문 안의 if보다 for문의 where를 선호하는 규칙
force_cast: force cast를 지양 하는 규칙 ex) NSNumber() as! Int
force_try: force try를 지양 하는 규칙 ex) try! a()
function_body_length: Function Body 라인수 체크 규칙
function_parameter_count: Function Parameter 개수 체크 규칙 Default 5개 이상(warning), 8개이상(error)
generic_type_name: Generic Name 규칙(대문자로 시작하고 길이는 1~20자 사이)
identifier_name: 변수 명 규칙 Default 최소길이 3(warning), 2(error), 최대길이 40(warning), 60(error), camelCase 지향
implicit_getter: Getter만 사용 하는 경우 암시적 지향 규칙
inclusive_language: 인종 차별 단어 지양 규칙
invalid_swiftlint_command: Swiftlint 명령 체크 규칙
is_disjoint: Set.intersection(_:).isEmpty 보다 Set.isDisjoint(with:)을 선호 하는 규칙
large_tuple: 튜플 멤버 변수 개수 체크 규칙 Default 2(warning), 3(error)
leading_whitespace: 파일 시작 부분 공백 체크 규칙
legacy_cggeometry_functions: 레거시 함수보다 구조체 확장 속성 및 메서드 선호 규칙 ex) CGRectGetWidth(rect) -> rect.width
legacy_constant: 레거시 전역 상수보다 구조체 범위 상수가 선호 규칙 ex) CGPointZero -> CGPoint.zero
legacy_constructor: 레거시 편의 함수보다 Swift 생성자가 선호 규칙 ex) CGPointMake(10,10) -> CGPoint(x: 10, y: 10)
legacy_hashing: hashValue 대신 hash(into:) 함수를 사용 선호 규칙
legacy_nsgeometry_functions: 레거시 함수보다 구조체 확장 속성 및 메서드 선호 규칙 ex) NSWidth(rect) -> rect.width
legacy_random: Legacy Random 지양 규칙 ex) arc4random() -> Int.random(in: 0..<10)
line_length: Column 길이 규칙 Default 120(warning) 200(error)
mark: Mark 주석 체크 규칙
multiple_closures_with_trailing_closure: 둘 이상의 클로저 인수를 전달할 때 후행 클로저 구문 지양 규칙
nesting: 중첩 체크 규칙
no_fallthrough_only: Fallthrough를 사용 할 때 한줄이상의 다른구문 포함 지향 규칙
no_space_in_method_call: 메소드 호출시 공백 지양 규칙 ex) foo () -> foo()
notification_center_detachment: Notification Center observer는 deinit에서만 remove해야 하는 규칙
ns_number_init_as_function_reference: NSNumber Init as Function Reference ex) NSNumber.init -> NSNumber.init(value:)
nsobject_prefer_isequal: NSObject 하위 클래스는 == 대신 isEqual을 구현해야 하는 규칙
opening_brace: 여는 중괄호 앞에는 단일 공백이 있어야 하며 선언과 같은 줄에 있어야 하는 규칙
operator_whitespace: 연산자를 정의할 때 연산자를 단일 공백으로 묶어야 하는 규칙
orphaned_doc_comment: Doc Comment는 선언에 첨부 해야하는 규칙
private_over_fileprivate: Fileprivate 보다 Private를 지향 하는 규칙
private_unit_test: 비공개로 표시된 단위 테스트는 자동으로 건너뛰는 규칙
protocol_property_accessors_order: 프로토콜 속성 접근자 순서 규칙 ex) { set get } -> { get set }
reduce_boolean: Reduce Boolean(Prefer using .allSatisfy() or .contains() over reduce(true) or reduce(false))
redundant_discardable_let: 함수의 결과를 버릴 때 let _ = foo() 보다 _ = foo()를 선호 하는 규칙
redundant_objc_attribute: @objc 속성 중복 체크 규칙
redundant_optional_initialization: 변수 선언시 중복 optional 지양 규칙 ex) var foo: Int? = nil -> var foo: Int?
redundant_set_access_control: 속성 설정자 액세스 수준이 변수 액세스 수준과 동일한 경우 명시적으로 표시 지양 규칙
redundant_string_enum_value: 문자열 열거형 값은 열거형 이름과 같으면 생략할 수 있습니다. ex) case name = "name" -> case name
redundant_void_return: 함수 선언에서 Void를 반환 중복 지양 정책
return_arrow_whitespace: 반환 화살표와 반환 유형은 단일 공백 또는 별도의 줄로 구분해야 하는 규칙
self_in_property_initialization: self refers to the unapplied NSObject.self() method, which is likely not expected; make the variable lazy to be able to refer to the current instance or use ClassName.self
shorthand_operator: 작업을 수행하고 할당하는 것보다 단축 연산자(+=, -=, *=, /=)를 선호 하는 규칙 ex) foo = foo * 1 -> foo *= 1
statement_position: else와 catch는 같은 줄에 있어야 하며 이전 선언 다음에는 한 칸 뒤에 있어야 하는 규칙
superfluous_disable_command: 비활성화된 규칙이 비활성화된 영역에서 위반을 유발하지 않았을 경우 SwiftLint 'disable' 명령은 불필요규칙
switch_case_alignment: Switch 및 Case 문 정렬 규칙
syntactic_sugar: Syntactic Sugar 구문 선호 규칙 ex) Array -> [String]
todo: TODO 및 FIXME 체크 규칙
trailing_comma: array와 dictionary의 쉼표 규칙
trailing_newline: 파일 끝에는 단일 줄바꿈만 있어야 하는 규칙
trailing_semicolon: 라인 후행 세미콜론 지양 규칙
trailing_whitespace: 라인 뒤에 공백이 있어서는 안 되는 규칙
type_body_length: Type Body 길이 체크 ex) class struct Default 250(warning), 350(error)
type_name: Type Name 체크 ex) 최소길이 3(warning), 0(error), 최대길이 40(warning), 1000(error)
unavailable_condition: 본문이 비어 있는 경우 #available/#unavailable 대신 #unavailable/#available 지향 규칙
unneeded_break_in_switch: switch 문에 불필요한 break 지양 규칙
unneeded_override: 슈퍼 호출 외에는 아무것도 하지 않는 재정의된 함수 지양 규칙
unneeded_synthesized_initializer: 자동으로 init 되는 기본 또는 멤버별 초기화 수동 지양 규칙
unused_closure_parameter: 클로저에서 사용되지 않는 매개변수는 _로 지향 규칙
unused_control_flow_label: 사용하지 않는 제어 흐름 레이블을 제거 규칙
unused_enumerated: 인덱스나 아이템이 사용되지 않을 때 .enumerated() 지양 규칙
unused_optional_binding: let _ = 보단 != nil 지향 규칙
unused_setter_value: 사용 되지 않는 Setter 지양 규칙
valid_ibinspectable: @IBInspectable은 변수에만 적용, 해당 유형이 명시적이어야 하는 규칙
vertical_parameter_alignment: 함수 매개변수 수직으로 정렬 체크 규칙
vertical_whitespace: Vertical 빈줄 한줄 제한 규칙
void_function_in_ternary: Void 함수를 호출하기 위해 삼항을 사용하는 것 지양 규칙
void_return: Void Return 지양 규칙
xctfail_message: XCTFail 호출에는 어설션에 대한 설명이 포함 지향 규칙
