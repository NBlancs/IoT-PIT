```mermaid
flowchart LR
    %% Registration Phase
    subgraph RP[Registration Phase]
        R1[Capture Student Face Images] --> R2[Extract Face Encodings]
        R2 --> R3[Store in Face Database: Name + School ID + Encoding]
    end

    %% Attendance Phase
    subgraph AP[Attendance Phase]
        A1[ESP32-CAM with Camera Module] -->|Captures Image| A2[Wi-Fi Network]
        A2 -->|HTTP POST Request| A3[Python Server Flask/FastAPI]
        A3 -->|Face Detection & Encoding| A4[OpenCV + face_recognition]
        A4 -->|Match with Database| A5[Face Database: Name + School ID + Encoding]
        A5 -->|Log with Timestamp| A6[Attendance Database/CSV: Name + School ID + Time]
        A6 -->|Optional| A7[Real-time Dashboard or Mobile App]
    end

    %% Arrange them side by side
    RP --- AP

    %% Styling
    style RP fill:#DDEEFF,stroke:#4477AA,stroke-width:2px
    style AP fill:#EFFFF0,stroke:#44AA77,stroke-width:2px

