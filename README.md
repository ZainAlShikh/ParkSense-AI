# ParkSense AI

## Setup 
```
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt

```

## Run order
1. `python roi_selector.py`
2. `python process_video.py`
3. `streamlit run app.py`

## Tunin
- Cars missed -> lower `CONFIDENCE`, use `yolov8s.pt`, raise `IMG_SIZE`
- Empty spaces flagged occupied -> raise `OVERLAP_THRESHOLD`
- Flickering -> raise `SMOOTH_WINDOW`
- Congestion thresholds -> `CONGESTION_LEVELS`
