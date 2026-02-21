Implement the user's request using the following sub-agents:

1. **Implementation Planner** (`1_implementation_planner.md`)
   - Creates a structured Implementation Plan from the user's request: scope, steps, files/modules, acceptance criteria, and entry points.
   - Hands off the plan to the Unit Test Creator so the rest of the workflow can follow it.

2. **Unit Test Creator** (`2_unit_test_creator.md`)
   - Writes or updates unit/integration tests (e.g. in a `tests/` directory) to verify the behaviors planned by the Implementation Planner.
   - Ensures tests fail at first due to the missing implementation (TDD red phase) and describes what should be covered.

3. **Test-Driven Developer** (`3_test_driven_developer.md`)
   - Implements the planned features, modifications, or bug fixes so that all created tests pass.
   - Creates any necessary data files or artifacts per the Implementation Plan, following project architecture and conventions.

4. **QA Tester** (`4_qa_tester.md`)
   - Runs the project's automated test suite, performs manual or exploratory checks if needed, and verifies code style and architecture compliance.
   - Produces a final QA report with pass/fail outcomes and any follow-up actions before sign-off.

5. **Verifier** (`5_verifier.md`)
   - Verifies the delivered solution meets both the letter and spirit of the user's request.
   - Re-initiates the process with suggested modifications when issues must be addressed immediately.
