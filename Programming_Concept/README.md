!!! before do check with GPT:

is that anything i miss out?:
and any thing i should split them more detail category?:


# Folder Structure
```text
Programming_Concepts/

├── README.md

├── 0000_Getting_Started/
│   ├── 0001_Installing_a_Compiler.md
│   ├── 0002_Your_First_Program.md
│   ├── 0003_How_to_Run_a_Program.md
│   ├── 0004_Common_Beginner_Tool_Setup.md
│   └── 0005_Hello_World_Explained.md

├── 0001_Introduction_to_Programming/
│   └── 0001_Fundamentals/
│       ├── 0001_What_is_Programming.md
│       ├── 0002_How_a_Program_Works.md
│       ├── 0003_Programming_Languages_Overview.md
│       └── 0004_Compilation_vs_Interpretation.md

├── 0002_Basic_Data_and_Values/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Variables.md
│   │   ├── 0002_Constants.md
│   │   └── 0003_Literals.md
│   ├── 0002_Data_Types/
│   │   ├── 0001_Primitive_Data_Types.md
│   │   ├── 0002_Non_Primitive_Data_Types.md
│   │   ├── 0003_Type_Size_and_Range.md
│   │   ├── 0004_Signed_vs_Unsigned.md
│   │   └── 0005_Boolean_Type.md
│   └── 0003_Type_Conversion/
│       ├── 0001_Type_Casting.md
│       ├── 0002_Implicit_vs_Explicit_Conversion.md
│       ├── 0003_Type_Promotion.md
│       └── 0004_Overflow_in_Type_Conversion.md

├── 0003_Input_Output_and_Documentation/
│   ├── 0001_Input_Output/
│   │   ├── 0001_Input_and_Output.md
│   │   ├── 0002_Formatted_Output.md
│   │   ├── 0003_Input_Buffer_Issues.md
│   │   ├── 0004_Formatted_Input.md
│   │   ├── 0005_Escape_Sequences.md
│   │   ├── 0006_Input_Validation_Basics.md
│   │   ├── 0007_Getline_vs_Cin.md
│   │   ├── 0008_Stream_Manipulators.md
│   │   ├── 0009_Setw_Setprecision.md
│   │   └── 0010_Input_Failure_Recovery.md
│   ├── 0002_Documentation/
│   │   ├── 0001_Comments.md
│   │   └── 0002_Documenting_Code.md
│   └── 0003_Code_Style/
│       ├── 0001_Code_Style.md
│       └── 0002_Naming_Conventions.md

├── 0004_Operators_and_Expressions/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Assignment.md
│   │   ├── 0002_Expressions.md
│   │   ├── 0003_Operator_Precedence.md
│   │   └── 0004_Associativity.md
│   ├── 0002_Types_of_Operators/
│   │   ├── 0001_Arithmetic.md
│   │   ├── 0002_Modulus.md
│   │   ├── 0003_Compound_Assignment.md
│   │   ├── 0004_Comparison.md
│   │   ├── 0005_Logical.md
│   │   ├── 0006_Increment_Decrement.md
│   │   ├── 0007_Bitwise.md
│   │   ├── 0008_Bit_Shift.md
│   │   ├── 0009_Unary_Operators.md
│   │   └── 0010_Ternary_Operator.md
│   └── 0003_Advanced/
│       ├── 0001_Boolean_Algebra.md
│       ├── 0002_Short_Circuit_Evaluation.md
│       ├── 0003_Relational_vs_Equality.md
│       └── 0004_Expressions_vs_Statements.md

├── 0005_Decision_Making/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_If.md
│   │   ├── 0002_If_Else.md
│   │   ├── 0003_Else_If_Ladder.md
│   │   └── 0004_Nested_If.md
│   └── 0002_Types/
│       ├── 0001_Switch.md
│       └── 0002_Switch_vs_If_Else.md

├── 0006_Loops_and_Control_Flow/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_For_Loop.md
│   │   ├── 0002_While_Loop.md
│   │   ├── 0003_Do_While_Loop.md
│   │   ├── 0004_Nested_Loops.md
│   │   ├── 0005_Infinite_Loops.md
│   │   ├── 0006_Counter_Controlled_Loop.md
│   │   └── 0007_Sentinel_Controlled_Loop.md
│   └── 0002_Control_Statements/
│       ├── 0001_Break.md
│       ├── 0002_Continue.md
│       └── 0003_Return_in_Control_Flow.md

├── 0007_Functions_and_Scope/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Function_Basics.md
│   │   ├── 0002_Declaration_vs_Definition.md
│   │   ├── 0003_Function_Prototypes.md
│   │   └── 0004_Main_Function.md
│   ├── 0002_Parameters_and_Return/
│   │   ├── 0001_Parameters.md
│   │   ├── 0002_Return_Values.md
│   │   ├── 0003_Pass_by_Value_vs_Reference.md
│   │   └── 0004_Return_by_Value_vs_Return_by_Reference.md
│   ├── 0003_Variables_and_Scope/
│   │   ├── 0001_Local_vs_Global.md
│   │   ├── 0002_Scope.md
│   │   └── 0003_Lifetime.md
│   └── 0004_Advanced/
│       ├── 0001_Default_Arguments.md
│       ├── 0002_Function_Overloading.md
│       ├── 0003_Inline_Functions.md
│       ├── 0004_Recursion.md
│       ├── 0005_Function_Call_Stack.md
│       ├── 0006_Function_Side_Effects.md
│       └── 0007_Function_Prototype_Mismatch.md

├── 0008_Arrays_and_Strings/
│   ├── 0001_Arrays/
│   │   ├── 0001_Declaration.md
│   │   ├── 0002_Basic_Arrays.md
│   │   ├── 0003_Multidimensional.md
│   │   ├── 0004_Indexing.md
│   │   ├── 0005_Traversal.md
│   │   ├── 0006_Operations.md
│   │   ├── 0007_Insertion_Deletion.md
│   │   ├── 0008_Searching.md
│   │   ├── 0009_Passing_to_Functions.md
│   │   ├── 0010_Array_Initialization.md
│   │   ├── 0011_Array_Bounds.md
│   │   └── 0012_Array_vs_Vector.md
│   └── 0002_Strings/
│       ├── 0001_Characters.md
│       ├── 0002_C_Style_Strings.md
│       ├── 0003_String_Object.md
│       ├── 0004_Comparison.md
│       ├── 0005_Traversal.md
│       ├── 0006_Operations.md
│       ├── 0007_Conversion.md
│       ├── 0008_String_Input_and_Output.md
│       ├── 0009_String_Length.md
│       ├── 0010_Substring.md
│       ├── 0011_ASCII_and_Character_Codes.md
│       ├── 0012_String_vs_Character_Array.md
│       ├── 0013_Empty_String.md
│       └── 0014_Common_String_Functions.md

├── 0009_User_Defined_Types/
│   └── 0001_Fundamentals/
│       ├── 0001_Structure.md
│       ├── 0002_Union.md
│       ├── 0003_Enumeration.md
│       ├── 0004_Typedef.md
│       ├── 0005_Using_Alias.md
│       └── 0006_Enum_Class.md

├── 0010_Memory_and_Pointers/
│   ├── 0001_Memory_Basics/
│   │   ├── 0001_Memory_Addresses.md
│   │   ├── 0002_Stack_vs_Heap.md
│   │   ├── 0003_Memory_Layout_Overview.md
│   │   └── 0004_RAII.md
│   ├── 0002_References/
│   │   ├── 0001_References.md
│   │   └── 0002_Reference_vs_Pointer.md
│   ├── 0003_Pointer_Basics/
│   │   ├── 0001_Basic.md
│   │   ├── 0002_Address_and_Dereference.md
│   │   ├── 0003_Pointer_Arithmetic.md
│   │   ├── 0004_Pointer_and_Array.md
│   │   ├── 0005_Passing_Pointers.md
│   │   ├── 0006_Null.md
│   │   ├── 0007_Wild.md
│   │   ├── 0008_Dangling.md
│   │   ├── 0009_Void.md
│   │   ├── 0010_Pointer_to_Pointer.md
│   │   ├── 0011_Const_Pointer.md
│   │   ├── 0012_Pointer_to_Const.md
│   │   ├── 0013_Array_of_Pointers.md
│   │   ├── 0014_Function_Pointers.md
│   │   └── 0015_Pointer_vs_Array.md
│   ├── 0004_Dynamic_Memory/
│   │   ├── 0001_Dynamic_Memory.md
│   │   ├── 0002_New_and_Delete.md
│   │   ├── 0003_Memory_Leaks.md
│   │   ├── 0004_Double_Delete.md
│   │   ├── 0005_Use_After_Free.md
│   │   ├── 0006_Null_Pointer_Dereference.md
│   │   └── 0007_Uninitialized_Pointer.md
│   ├── 0005_Common_Problems/
│   │   └── 0001_Common_Mistakes.md
│   └── 0006_Modern_Cpp_Memory/
│       ├── 0001_Smart_Pointers.md
│       ├── 0002_Unique_Ptr.md
│       ├── 0003_Shared_Ptr.md
│       └── 0004_Weak_Ptr.md

├── 0011_File_Handling_and_Program_Organization/
│   ├── 0001_File_Handling/
│   │   ├── 0001_Introduction.md
│   │   ├── 0002_Open_and_Close.md
│   │   ├── 0003_File_Modes.md
│   │   ├── 0004_Reading.md
│   │   ├── 0005_Writing.md
│   │   ├── 0006_Appending.md
│   │   ├── 0007_Text_vs_Binary.md
│   │   ├── 0008_End_of_File.md
│   │   ├── 0009_Error_Checking.md
│   │   ├── 0010_File_Paths.md
│   │   ├── 0011_CSV_and_Structured_Text_Files.md
│   │   ├── 0012_File_Read_Write_Patterns.md
│   │   └── 0013_File_Stream_States.md
│   └── 0002_Program_Structure/
│       ├── 0001_Preprocessor_Directives.md
│       ├── 0002_Header_Files.md
│       ├── 0003_Source_vs_Header.md
│       ├── 0004_Modular_Programming.md
│       ├── 0005_Include_Guards.md
│       ├── 0006_Namespace.md
│       └── 0007_Multiple_Source_Files_Workflow.md

├── 0012_Object_Oriented_Programming/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Object_Oriented_Programming_Overview.md
│   │   ├── 0002_Class_and_Object.md
│   │   ├── 0003_Encapsulation.md
│   │   ├── 0004_Abstraction.md
│   │   └── 0005_Procedural_vs_Object_Oriented.md
│   ├── 0002_Class_Design/
│   │   ├── 0001_Access_Specifiers.md
│   │   ├── 0002_This_Pointer.md
│   │   ├── 0003_Friend_Function_and_Class.md
│   │   ├── 0004_Setters_and_Getters.md
│   │   ├── 0005_Static_Members.md
│   │   ├── 0006_Const_Member_Function.md
│   │   ├── 0007_Constructor_Initialization_List.md
│   │   └── 0008_Mutable_and_Const_Objects.md
│   ├── 0003_Object_Lifecycle/
│   │   ├── 0001_Constructors.md
│   │   ├── 0002_Constructor_Overloading.md
│   │   ├── 0003_Destructors.md
│   │   ├── 0004_Copy_Constructor.md
│   │   ├── 0005_Copy_Assignment_Operator.md
│   │   ├── 0006_Move_Semantics.md
│   │   ├── 0007_Rule_of_Three.md
│   │   ├── 0008_Rule_of_Five.md
│   │   ├── 0009_Rule_of_Zero.md
│   │   └── 0010_Shallow_Copy_vs_Deep_Copy.md
│   ├── 0004_Inheritance_and_Relationships/
│   │   ├── 0001_Inheritance.md
│   │   ├── 0002_Types_of_Inheritance.md
│   │   ├── 0003_Method_Overriding.md
│   │   ├── 0004_Composition.md
│   │   ├── 0005_Association.md
│   │   ├── 0006_Aggregation.md
│   │   ├── 0007_Object_Relationships.md
│   │   ├── 0008_Multiple_Inheritance.md
│   │   ├── 0009_Is_A_vs_Has_A.md
│   │   ├── 0010_When_to_Use_Inheritance.md
│   │   ├── 0011_When_to_Use_Composition.md
│   │   └── 0012_Access_Control_in_Inheritance.md
│   ├── 0005_Polymorphism/
│   │   ├── 0001_Function_Overloading.md
│   │   ├── 0002_Operator_Overloading.md
│   │   ├── 0003_Virtual_Functions.md
│   │   ├── 0004_Abstract_Class.md
│   │   ├── 0005_Compile_Time_vs_Runtime_Polymorphism.md
│   │   ├── 0006_Pure_Virtual_Function.md
│   │   ├── 0007_Virtual_Destructor.md
│   │   ├── 0008_Dynamic_Binding.md
│   │   └── 0009_Object_Slicing.md
│   └── 0006_Design_Guidelines/
│       ├── 0001_Interface_Thinking.md
│       └── 0002_Const_Correctness.md

├── 0013_Basic_Data_Structures/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Data_Structures_Overview.md
│   │   ├── 0002_Abstract_Data_Type.md
│   │   ├── 0003_Static_vs_Dynamic_Data_Structure.md
│   │   └── 0004_Array_as_Data_Structure.md
│   ├── 0002_Linear_Data_Structures/
│   │   ├── 0001_Array_vs_Linked_List.md
│   │   ├── 0002_Linked_List/
│   │   │   ├── 0001_Singly_Linked_List.md
│   │   │   ├── 0002_Doubly_Linked_List.md
│   │   │   ├── 0003_Circular_Linked_List.md
│   │   │   └── 0004_Linked_List_Operations.md
│   │   ├── 0003_Stack/
│   │   │   ├── 0001_Stack_Concept.md
│   │   │   ├── 0002_Stack_Operations.md
│   │   │   ├── 0003_Array_Based_Stack.md
│   │   │   └── 0004_Linked_List_Based_Stack.md
│   │   ├── 0004_Queue/
│   │   │   ├── 0001_Queue_Concept.md
│   │   │   ├── 0002_Queue_Operations.md
│   │   │   ├── 0003_Circular_Queue.md
│   │   │   ├── 0004_Array_Based_Queue.md
│   │   │   └── 0005_Linked_List_Based_Queue.md
│   │   ├── 0005_Deque.md
│   │   └── 0006_Priority_Queue.md
│   └── 0003_Comparison/
│       ├── 0001_Array_vs_Vector.md
│       ├── 0002_Stack_vs_Queue.md
│       └── 0003_Static_vs_Dynamic_Memory_Usage.md

├── 0014_Algorithms_and_Problem_Solving/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Algorithms.md
│   │   ├── 0002_Tracing_an_Algorithm.md
│   │   ├── 0003_Recursion_vs_Iteration.md
│   │   ├── 0004_Time_and_Space_Complexity.md
│   │   ├── 0005_Brute_Force.md
│   │   ├── 0006_Algorithm_Correctness.md
│   │   └── 0007_Input_Output_Tracing.md
│   ├── 0002_Searching/
│   │   ├── 0001_Linear_Search.md
│   │   └── 0002_Binary_Search.md
│   ├── 0003_Sorting/
│   │   ├── 0001_Bubble_Sort.md
│   │   ├── 0002_Selection_Sort.md
│   │   ├── 0003_Insertion_Sort.md
│   │   ├── 0004_Merge_Sort.md
│   │   ├── 0005_Quick_Sort.md
│   │   └── 0006_Stable_vs_Unstable_Sorting.md
│   ├── 0004_Strategies/
│   │   ├── 0001_Greedy_Algorithm.md
│   │   ├── 0002_Divide_and_Conquer.md
│   │   ├── 0003_Backtracking.md
│   │   └── 0004_Dynamic_Programming_Introduction.md
│   ├── 0005_Analysis/
│   │   ├── 0001_Big_O_Notation.md
│   │   └── 0002_Best_Worst_and_Average_Case.md
│   ├── 0006_Problem_Patterns/
│   │   ├── 0001_Two_Pointers.md
│   │   ├── 0002_Sliding_Window.md
│   │   ├── 0003_Prefix_Sum.md
│   │   ├── 0004_Binary_Search_on_Answer.md
│   │   ├── 0005_Recursion_Tree_Basics.md
│   │   ├── 0006_Frequency_Counting.md
│   │   ├── 0007_Hashing_for_Lookups.md
│   │   └── 0008_Simulation.md
│   └── 0007_Basic_Math_Tools/
│       ├── 0001_Prime_Check_Basics.md
│       ├── 0002_GCD_and_LCM.md
│       ├── 0003_Modular_Arithmetic_Basics.md
│       └── 0004_Powers_and_Logarithms_in_Algorithms.md

├── 0015_Number_Systems_and_Data_Representation/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Bits_and_Bytes.md
│   │   ├── 0002_Place_Value.md
│   │   ├── 0003_Base_or_Radix.md
│   │   └── 0004_Number_System_Overview.md
│   ├── 0002_Types/
│   │   ├── 0001_Binary.md
│   │   ├── 0002_Decimal.md
│   │   ├── 0003_Octal.md
│   │   └── 0004_Hexadecimal.md
│   ├── 0003_Number_Conversions/
│   │   ├── 0001_Decimal_to_Binary.md
│   │   ├── 0002_Binary_to_Decimal.md
│   │   ├── 0003_Decimal_to_Hexadecimal.md
│   │   ├── 0004_Hexadecimal_to_Decimal.md
│   │   ├── 0005_Binary_to_Hexadecimal.md
│   │   ├── 0006_Hexadecimal_to_Binary.md
│   │   ├── 0007_Binary_to_Octal.md
│   │   ├── 0008_Octal_to_Binary.md
│   │   └── 0009_Quick_Conversion_Methods.md
│   ├── 0004_Binary_Arithmetic/
│   │   ├── 0001_Binary_Addition.md
│   │   ├── 0002_Binary_Subtraction.md
│   │   ├── 0003_Binary_Multiplication.md
│   │   └── 0004_Binary_Division.md
│   ├── 0005_Signed_Number_Representation/
│   │   ├── 0001_Signed_vs_Unsigned.md
│   │   ├── 0002_Ones_Complement.md
│   │   ├── 0003_Twos_Complement.md
│   │   └── 0004_Range_of_Values.md
│   └── 0006_Data_Representation/
│       ├── 0001_ASCII_and_Unicode.md
│       ├── 0002_Integer_Overflow_and_Underflow.md
│       ├── 0003_Fixed_Point_vs_Floating_Point.md
│       ├── 0004_Character_Encoding.md
│       ├── 0005_Endianness.md
│       └── 0006_Boolean_Representation.md

├── 0016_Debugging_and_Testing/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Debugging.md
│   │   ├── 0002_Dry_Run.md
│   │   ├── 0003_Test_Cases.md
│   │   └── 0004_Breakpoints.md
│   ├── 0002_Testing/
│   │   ├── 0001_Unit_Testing.md
│   │   ├── 0002_Assertions.md
│   │   ├── 0003_Boundary_Value_Testing.md
│   │   └── 0004_Normal_and_Edge_Cases.md
│   └── 0003_Test_Design/
│       ├── 0001_Happy_Path.md
│       ├── 0002_Edge_Cases.md
│       ├── 0003_Invalid_Input_Cases.md
│       └── 0004_Test_Case_Thinking.md

├── 0017_Errors_and_Exception_Handling/
│   ├── 0001_Types_of_Errors/
│   │   ├── 0001_Syntax_Errors.md
│   │   ├── 0002_Logic_Errors.md
│   │   ├── 0003_Runtime_Errors.md
│   │   ├── 0004_Compile_Time_Errors.md
│   │   ├── 0005_Linker_Errors.md
│   │   └── 0006_Warnings.md
│   └── 0002_Error_Handling/
│       ├── 0001_Exception_Handling.md
│       ├── 0002_Try_Catch.md
│       ├── 0003_Throw.md
│       ├── 0004_Input_Validation.md
│       ├── 0005_Defensive_Programming.md
│       ├── 0006_Exception_Safety_Basics.md
│       ├── 0007_Stack_Unwinding.md
│       ├── 0008_When_to_Use_Exceptions.md
│       ├── 0009_When_Not_to_Use_Exceptions.md
│       └── 0010_Custom_Exceptions.md

├── 0018_Program_Design/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Pseudocode.md
│   │   ├── 0002_Flowcharts.md
│   │   └── 0003_Structured_Programming.md
│   ├── 0002_Design_Principles/
│   │   ├── 0001_Problem_Decomposition.md
│   │   ├── 0002_Top_Down_vs_Bottom_Up.md
│   │   ├── 0003_Code_Readability.md
│   │   ├── 0004_Modular_Design.md
│   │   ├── 0005_Stepwise_Refinement.md
│   │   ├── 0006_Cohesion_and_Coupling.md
│   │   ├── 0007_Single_Responsibility_Idea.md
│   │   ├── 0008_Separation_of_Concerns.md
│   │   └── 0009_Reusability.md
│   └── 0003_Problem_Solving_Workflow/
│       ├── 0001_Understand_the_Problem.md
│       ├── 0002_Break_the_Problem_Down.md
│       ├── 0003_Design_Before_Code.md
│       ├── 0004_Test_with_Sample_Input.md
│       └── 0005_Refine_and_Improve.md

├── 0019_Advanced_Data_Structures/
│   ├── 0001_Trees/
│   │   ├── 0001_Basic_Tree.md
│   │   ├── 0002_Binary_Tree.md
│   │   ├── 0003_Tree_Traversal.md
│   │   ├── 0004_Binary_Search_Tree_Operations.md
│   │   ├── 0005_AVL_Tree_Introduction.md
│   │   ├── 0006_Heap_vs_Binary_Search_Tree.md
│   │   └── 0007_Tree_Height_and_Balance.md
│   ├── 0002_Binary_Search_Tree.md
│   ├── 0003_Heap.md
│   ├── 0004_Hash_Tables/
│   │   ├── 0001_Basic_Hashing.md
│   │   ├── 0002_Collision_Handling.md
│   │   └── 0003_Hash_Function_Basics.md
│   ├── 0005_Graph/
│   │   ├── 0001_Basic_Graph.md
│   │   ├── 0002_Types_of_Graphs.md
│   │   ├── 0003_Breadth_First_Search.md
│   │   ├── 0004_Depth_First_Search.md
│   │   ├── 0005_Shortest_Path_Introduction.md
│   │   ├── 0006_Topological_Sort_Introduction.md
│   │   └── 0007_Adjacency_List_vs_Adjacency_Matrix.md
│   └── 0006_Comparison/
│       ├── 0001_BST_vs_Heap.md
│       ├── 0002_Map_vs_Unordered_Map.md
│       └── 0003_DFS_vs_BFS.md

├── 0020_Software_Development/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Version_Control.md
│   │   ├── 0002_Build_Process.md
│   │   ├── 0003_Software_Development_Life_Cycle.md
│   │   └── 0004_Debug_vs_Release.md
│   ├── 0002_Core_Concepts/
│   │   ├── 0001_Source_Code_vs_Object_Code.md
│   │   ├── 0002_Libraries.md
│   │   ├── 0003_Compiler.md
│   │   ├── 0004_Linker.md
│   │   ├── 0005_Loader.md
│   │   └── 0006_Static_vs_Dynamic_Libraries.md
│   ├── 0003_Tools/
│   │   ├── 0001_Command_Line.md
│   │   ├── 0002_Integrated_Development_Environment.md
│   │   └── 0003_Debugger.md
│   └── 0004_Project_Workflow/
│       ├── 0001_Project_Folder_Structure.md
│       ├── 0002_Build_Errors_vs_Runtime_Errors.md
│       ├── 0003_Debugging_Workflow.md
│       └── 0004_Readme_and_Documentation_Basics.md

├── 0021_Basic_Security/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Input_Validation_vs_Input_Sanitization.md
│   │   ├── 0002_Buffer_Overflow.md
│   │   ├── 0003_Integer_Overflow.md
│   │   ├── 0004_Secure_Coding_Principles.md
│   │   └── 0005_Principle_of_Least_Privilege.md
│   └── 0002_Common_Attacks/
│       ├── 0001_Common_Input_Attacks.md
│       ├── 0002_Password_Handling.md
│       ├── 0003_SQL_Injection_Basics.md
│       └── 0004_Command_Injection_Basics.md

├── 0022_Concurrency/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Threads.md
│   │   ├── 0002_Thread_Lifecycle.md
│   │   ├── 0003_Critical_Section.md
│   │   └── 0004_Thread_Safety.md
│   ├── 0002_Common_Problems/
│   │   ├── 0001_Race_Conditions.md
│   │   └── 0002_Deadlock.md
│   └── 0003_Synchronization_and_Solutions/
│       ├── 0001_Mutex_Locks.md
│       ├── 0002_Semaphore.md
│       ├── 0003_Basic_Synchronization_Concepts.md
│       ├── 0004_Producer_Consumer_Problem.md
│       ├── 0005_Condition_Variables.md
│       └── 0006_Read_Write_Locks.md

├── 0023_Computer_Fundamentals/
│   ├── 0001_How_Programs_Run/
│   │   ├── 0001_How_Code_Becomes_a_Program.md
│   │   ├── 0002_Source_Code_to_Executable.md
│   │   ├── 0003_Compiler_Interpreter_and_Assembler.md
│   │   └── 0004_Machine_Code_vs_Assembly_vs_High_Level_Code.md
│   ├── 0002_Computer_Architecture_Basics/
│   │   ├── 0001_CPU_Memory_and_Storage.md
│   │   ├── 0002_Instruction_Cycle.md
│   │   ├── 0003_Register_Basics.md
│   │   └── 0004_Memory_Addressing_Basics.md
│   ├── 0003_Operating_System_Basics/
│   │   ├── 0001_Basic_Operating_System_Role.md
│   │   ├── 0002_System_Calls_Basics.md
│   │   ├── 0003_Process_vs_Thread.md
│   │   └── 0004_RAM_vs_ROM.md
│   └── 0004_Command_Line/
│       └── 0001_Command_Line_Basics.md

├── 0024_Cpp_Standard_Library/
│   ├── 0001_Containers/
│   │   ├── 0001_Vector.md
│   │   ├── 0002_List.md
│   │   ├── 0003_Deque.md
│   │   ├── 0004_Stack.md
│   │   ├── 0005_Queue.md
│   │   ├── 0006_Priority_Queue.md
│   │   ├── 0007_Set.md
│   │   ├── 0008_Map.md
│   │   ├── 0009_Unordered_Set.md
│   │   └── 0010_Unordered_Map.md
│   ├── 0002_Utilities/
│   │   ├── 0001_Pair.md
│   │   ├── 0002_Auto_Keyword.md
│   │   ├── 0003_Custom_Comparator.md
│   │   ├── 0004_Function_Object_Functor.md
│   │   └── 0005_Predicate_Basics.md
│   ├── 0003_Iterators/
│   │   ├── 0001_Iterator.md
│   │   ├── 0002_Iterator_Categories.md
│   │   └── 0003_Iterator_Invalidation.md
│   ├── 0004_Algorithms/
│   │   ├── 0001_Algorithm_Header.md
│   │   ├── 0002_Sort.md
│   │   ├── 0003_Find.md
│   │   ├── 0004_Count.md
│   │   ├── 0005_Binary_Search.md
│   │   └── 0006_Lower_Bound_and_Upper_Bound.md
│   └── 0005_Strings/
│       └── 0001_String.md

├── 0025_Modern_Cpp/
│   ├── 0001_Core_Features/
│   │   ├── 0001_Const.md
│   │   ├── 0002_References.md
│   │   ├── 0003_Auto.md
│   │   ├── 0004_Range_Based_For.md
│   │   ├── 0005_Enum_Class.md
│   │   └── 0006_Lambda_Basics.md
│   ├── 0002_Resource_Management/
│   │   ├── 0001_Move_vs_Copy.md
│   │   ├── 0002_RAII.md
│   │   └── 0003_Smart_Pointers_Usage.md
│   └── 0003_Best_Practices/
│       └── 0001_Modern_Cpp_Best_Practices.md

├── 0026_Templates/
│   ├── 0001_Fundamentals/
│   │   ├── 0001_Function_Templates.md
│   │   ├── 0002_Class_Templates.md
│   │   └── 0003_Generic_Programming_Basics.md
│   └── 0002_Advanced/
│       ├── 0001_Template_Specialization.md
│       └── 0002_STL_and_Templates_Relationship.md

└── 0027_Practice_and_Exercises/
    ├── 0001_Beginner_Problems/
    │   ├── 0001_Output_Basics.md
    │   ├── 0002_Variables_and_Input.md
    │   └── 0003_Simple_Calculations.md
    ├── 0002_Decision_Problems/
    │   ├── 0001_If_Problems.md
    │   ├── 0002_Switch_Problems.md
    │   └── 0003_Nested_Decision_Problems.md
    ├── 0003_Loop_Problems/
    │   ├── 0001_For_Loop_Problems.md
    │   ├── 0002_While_Loop_Problems.md
    │   └── 0003_Nested_Loop_Problems.md
    ├── 0004_Function_Problems/
    │   ├── 0001_Basic_Function_Problems.md
    │   ├── 0002_Parameter_and_Return_Problems.md
    │   └── 0003_Recursion_Problems.md
    ├── 0005_Array_Problems/
    │   ├── 0001_Array_Traversal_Problems.md
    │   ├── 0002_Searching_and_Counting.md
    │   └── 0003_Array_Manipulation_Problems.md
    ├── 0006_String_Problems/
    │   ├── 0001_String_Input_Problems.md
    │   ├── 0002_String_Traversal_Problems.md
    │   └── 0003_String_Operation_Problems.md
    ├── 0007_Pointer_Problems/
    │   ├── 0001_Basic_Pointer_Problems.md
    │   ├── 0002_Dynamic_Memory_Problems.md
    │   └── 0003_Pointer_and_Array_Problems.md
    ├── 0008_Linked_List_Problems/
    │   ├── 0001_Singly_Linked_List_Problems.md
    │   ├── 0002_Doubly_Linked_List_Problems.md
    │   └── 0003_Linked_List_Tracing.md
    └── 0009_Algorithm_Tracing_Problems/
        ├── 0001_Searching_Trace_Problems.md
        ├── 0002_Sorting_Trace_Problems.md
        └── 0003_Time_Complexity_Thinking_Problems.md
```
