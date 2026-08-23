# Presentation review checklist

This revision was checked against the comments from the earlier reviewed presentation and the latest requested changes.

## Earlier review comments

- Motivation gives concrete document examples and explains why text regions are useful.
- The task is defined as text-block detection, not semantic field classification.
- The work is framed as a preprocessing step for later OCR, NLP, or layout analysis.
- The challenge slide now explains why additional labels are costly instead of implying that FUNSD is unlabeled.
- Synthetic generation explicitly starts from an annotated source dataset.
- The generation slide states that document layout and non-text structure are preserved.
- Faster R-CNN is explained with a simple input, backbone, RPN, and refinement flow.
- A general teacher-student self-training slide appears before the ASTOD-specific adaptation.
- FUNSD details were corrected to claims supported by the FUNSD paper: 199 real, fully annotated scanned forms; noisy and varied appearance; 149 train and 50 test; word boxes and semantic entities.
- Unsupported claims about grayscale/black-and-white images or varying resolution were removed.
- Wikipedia is named as the source of inserted synthetic text.
- Parameter choice is now contextualized by related literature, while the exact thesis values are clearly identified as the result of preliminary sweeps.
- Time-development results remain graphs; final comparisons are primarily tables or compact number summaries.
- The 10%, 25%, 50%, 75%, and 100% synthetic-data experiments are shown together.
- Inpainting and white-background examples are shown immediately before their result comparison.
- Main self-training results appear after setup and ablations are grouped near the end.
- Claims are kept cautious: self-training reduces the gap but does not replace real supervision.

## Latest requested changes

- Removed the four metric boxes from the challenge slide because those facts are explained more clearly on the following data and baseline slides.
- Clarified that FUNSD itself is fully annotated. The label problem is the cost of adding more real training pages.
- Made the self-training introduction general. The thesis-specific adaptation begins on the following ASTOD slide.
- Added literature context for the detector and optimizer family. The exact LR, momentum, and weight decay are still attributed to the thesis sweeps, not copied from another paper.
- Added a one-sentence experiment question to every main experiment slide.
- Removed the Gap row from the baseline table and stated the gap as a sentence below the table.
- The task and data slides use different real-form examples to avoid repeating the same image.
- Only two synthetic generation variants are shown: inpainting and white background.
- Replaced ambiguous wording such as pseudo-real with pseudo-labeled real pages or teacher-labeled real pages and explicitly defined the term.
- Enlarged the real-label experiment graph and reduced the surrounding text.
- No em dash characters are used in visible presentation text.
