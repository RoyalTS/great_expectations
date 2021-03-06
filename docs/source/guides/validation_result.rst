.. _validation_result:


Validation Results
===================

Validation results include information about each expectation that was validated and a ``statistics`` section that
describes the overall number of validated expectations and results.

For example:

::

    {
      "meta": {
        "data_asset_name": "data__dir/default/titanic",
        "expectation_suite_name": "default",
        "run_id": "2019-07-01T123434.12345Z"
      },
      "results": [
        {
          "expectation_config": {
            "expectation_type": "expect_column_values_to_have_odd_lengths",
            "kwargs": {
              "column": "Name",
              "result_format": "SUMMARY"
            }
          },
          "exception_info": {
            "exception_message": null,
            "exception_traceback": null,
            "raised_exception": false
          },
          "success": false,
          "result": {
            "partial_unexpected_index_list": [
              0,
              5,
              6,
              7,
              8,
              9,
              11,
              12,
              13,
              14,
              15,
              18,
              20,
              21,
              22,
              23,
              27,
              31,
              32,
              33
            ],
            "unexpected_count": 660,
            "unexpected_percent": 0.5026656511805027,
            "partial_unexpected_list": [
              "Allen, Miss Elisabeth Walton",
              "Anderson, Mr Harry",
              "Andrews, Miss Kornelia Theodosia",
              "Andrews, Mr Thomas, jr",
              "Appleton, Mrs Edward Dale (Charlotte Lamson)",
              "Artagaveytia, Mr Ramon",
              "Astor, Mrs John Jacob (Madeleine Talmadge Force)",
              "Aubert, Mrs Leontine Pauline",
              "Barkworth, Mr Algernon H",
              "Baumann, Mr John D",
              "Baxter, Mrs James (Helene DeLaudeniere Chaput)",
              "Beckwith, Mr Richard Leonard",
              "Behr, Mr Karl Howell",
              "Birnbaum, Mr Jakob",
              "Bishop, Mr Dickinson H",
              "Bishop, Mrs Dickinson H (Helen Walton)",
              "Bonnell, Miss Caroline",
              "Bowerman, Miss Elsie Edith",
              "Bradley, Mr George",
              "Brady, Mr John Bertram"
            ],
            "missing_percent": 0.0,
            "element_count": 1313,
            "unexpected_percent_nonmissing": 0.5026656511805027,
            "missing_count": 0
          }
        }
      ],
      "success": false,
      "statistics": {
        "evaluated_expectations": 1,
        "successful_expectations": 0,
        "unsuccessful_expectations": 1,
        "success_percent": 0
      }
    }
